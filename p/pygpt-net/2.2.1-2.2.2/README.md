# Comparing `tmp/pygpt_net-2.2.1.tar.gz` & `tmp/pygpt_net-2.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygpt_net-2.2.1.tar", max compression
+gzip compressed data, was "pygpt_net-2.2.2.tar", max compression
```

## Comparing `pygpt_net-2.2.1.tar` & `pygpt_net-2.2.2.tar`

### file list

```diff
@@ -1,844 +1,844 @@
--rwxr-xr-x   0        0        0    57370 2024-04-28 08:05:35.570679 pygpt_net-2.2.1/CHANGELOG.md
--rwxr-xr-x   0        0        0     1077 2024-02-01 17:53:56.362106 pygpt_net-2.2.1/LICENSE
--rwxr-xr-x   0        0        0   131486 2024-04-28 08:05:35.574680 pygpt_net-2.2.1/README.md
--rwxr-xr-x   0        0        0    13970 2024-02-19 21:38:20.920806 pygpt_net-2.2.1/icon.png
--rw-r--r--   0        0        0     2979 2024-04-28 08:05:35.578680 pygpt_net-2.2.1/pyproject.toml
--rwxr-xr-x   0        0        0    56352 2024-04-28 08:05:35.578680 pygpt_net-2.2.1/src/pygpt_net/CHANGELOG.txt
--rwxr-xr-x   0        0        0     1146 2024-02-01 17:53:56.366106 pygpt_net-2.2.1/src/pygpt_net/LICENSE
--rwxr-xr-x   0        0        0     1024 2024-04-28 08:05:35.578680 pygpt_net-2.2.1/src/pygpt_net/__init__.py
--rwxr-xr-x   0        0        0    14345 2024-04-17 01:35:30.422055 pygpt_net-2.2.1/src/pygpt_net/app.py
--rwxr-xr-x   0        0        0    14787 2024-04-11 03:43:59.058733 pygpt_net-2.2.1/src/pygpt_net/config.py
--rwxr-xr-x   0        0        0     3350 2024-02-24 01:55:58.445111 pygpt_net-2.2.1/src/pygpt_net/container.py
--rwxr-xr-x   0        0        0     5991 2024-04-28 08:05:35.578680 pygpt_net-2.2.1/src/pygpt_net/controller/__init__.py
--rw-r--r--   0        0        0     4662 2024-02-25 05:32:34.229344 pygpt_net-2.2.1/src/pygpt_net/controller/agent/__init__.py
--rw-r--r--   0        0        0     6829 2024-03-17 13:18:45.622350 pygpt_net-2.2.1/src/pygpt_net/controller/agent/flow.py
--rw-r--r--   0        0        0     8924 2024-04-27 07:58:32.750704 pygpt_net-2.2.1/src/pygpt_net/controller/assistant/__init__.py
--rw-r--r--   0        0        0    12703 2024-04-27 07:58:32.750704 pygpt_net-2.2.1/src/pygpt_net/controller/assistant/batch.py
--rw-r--r--   0        0        0    13203 2024-04-27 14:05:11.727541 pygpt_net-2.2.1/src/pygpt_net/controller/assistant/editor.py
--rw-r--r--   0        0        0    14001 2024-04-27 07:58:32.750704 pygpt_net-2.2.1/src/pygpt_net/controller/assistant/files.py
--rwxr-xr-x   0        0        0    14251 2024-04-27 14:05:11.727541 pygpt_net-2.2.1/src/pygpt_net/controller/assistant/store.py
--rw-r--r--   0        0        0    17258 2024-04-28 06:16:26.324027 pygpt_net-2.2.1/src/pygpt_net/controller/assistant/threads.py
--rwxr-xr-x   0        0        0    15463 2024-04-26 21:55:50.675598 pygpt_net-2.2.1/src/pygpt_net/controller/attachment.py
--rw-r--r--   0        0        0     5972 2024-03-20 16:01:43.275339 pygpt_net-2.2.1/src/pygpt_net/controller/audio/__init__.py
--rw-r--r--   0        0        0     3848 2024-03-09 00:22:17.287774 pygpt_net-2.2.1/src/pygpt_net/controller/calendar/__init__.py
--rw-r--r--   0        0        0     8585 2024-04-11 03:43:59.058733 pygpt_net-2.2.1/src/pygpt_net/controller/calendar/note.py
--rwxr-xr-x   0        0        0    12774 2024-03-15 15:31:21.786121 pygpt_net-2.2.1/src/pygpt_net/controller/camera.py
--rw-r--r--   0        0        0     1436 2024-01-13 16:28:42.715718 pygpt_net-2.2.1/src/pygpt_net/controller/chat/__init__.py
--rwxr-xr-x   0        0        0    11360 2024-04-23 23:11:13.256158 pygpt_net-2.2.1/src/pygpt_net/controller/chat/common.py
--rw-r--r--   0        0        0     2144 2024-03-15 15:31:21.786121 pygpt_net-2.2.1/src/pygpt_net/controller/chat/files.py
--rwxr-xr-x   0        0        0     6279 2024-03-26 17:12:51.286309 pygpt_net-2.2.1/src/pygpt_net/controller/chat/image.py
--rwxr-xr-x   0        0        0     9801 2024-03-15 15:31:21.786121 pygpt_net-2.2.1/src/pygpt_net/controller/chat/input.py
--rwxr-xr-x   0        0        0    10189 2024-04-26 21:55:50.675598 pygpt_net-2.2.1/src/pygpt_net/controller/chat/output.py
--rwxr-xr-x   0        0        0     9610 2024-04-25 00:06:58.371551 pygpt_net-2.2.1/src/pygpt_net/controller/chat/render.py
--rw-r--r--   0        0        0    12003 2024-04-28 06:16:26.324027 pygpt_net-2.2.1/src/pygpt_net/controller/chat/text.py
--rw-r--r--   0        0        0     3382 2024-04-11 20:50:24.189030 pygpt_net-2.2.1/src/pygpt_net/controller/chat/vision.py
--rw-r--r--   0        0        0     5292 2024-03-26 17:12:51.286309 pygpt_net-2.2.1/src/pygpt_net/controller/command.py
--rw-r--r--   0        0        0     4485 2024-04-26 21:55:50.675598 pygpt_net-2.2.1/src/pygpt_net/controller/config/__init__.py
--rw-r--r--   0        0        0        0 2024-01-08 20:36:28.054492 pygpt_net-2.2.1/src/pygpt_net/controller/config/field/__init__.py
--rwxr-xr-x   0        0        0     2422 2024-01-30 20:56:32.772879 pygpt_net-2.2.1/src/pygpt_net/controller/config/field/checkbox.py
--rw-r--r--   0        0        0     4863 2024-03-12 06:49:17.164785 pygpt_net-2.2.1/src/pygpt_net/controller/config/field/cmd.py
--rw-r--r--   0        0        0     3237 2024-04-27 14:05:11.727541 pygpt_net-2.2.1/src/pygpt_net/controller/config/field/combo.py
--rw-r--r--   0        0        0     6657 2024-03-12 06:49:17.164785 pygpt_net-2.2.1/src/pygpt_net/controller/config/field/dictionary.py
--rw-r--r--   0        0        0     3556 2024-03-15 15:31:21.786121 pygpt_net-2.2.1/src/pygpt_net/controller/config/field/input.py
--rw-r--r--   0        0        0     4580 2024-04-21 01:33:54.239765 pygpt_net-2.2.1/src/pygpt_net/controller/config/field/slider.py
--rw-r--r--   0        0        0     2337 2024-04-22 21:31:19.988317 pygpt_net-2.2.1/src/pygpt_net/controller/config/field/textarea.py
--rw-r--r--   0        0        0     7245 2024-04-24 02:39:32.054775 pygpt_net-2.2.1/src/pygpt_net/controller/config/placeholder.py
--rw-r--r--   0        0        0    29296 2024-04-28 06:16:26.324027 pygpt_net-2.2.1/src/pygpt_net/controller/ctx/__init__.py
--rw-r--r--   0        0        0     5434 2024-04-10 01:07:30.184635 pygpt_net-2.2.1/src/pygpt_net/controller/ctx/common.py
--rwxr-xr-x   0        0        0     7477 2024-04-24 05:19:32.002030 pygpt_net-2.2.1/src/pygpt_net/controller/ctx/extra.py
--rw-r--r--   0        0        0     2552 2024-01-25 22:43:11.543975 pygpt_net-2.2.1/src/pygpt_net/controller/ctx/summarizer.py
--rw-r--r--   0        0        0     7633 2024-04-26 21:55:50.675598 pygpt_net-2.2.1/src/pygpt_net/controller/debug/__init__.py
--rw-r--r--   0        0        0     1008 2023-12-31 03:09:04.107766 pygpt_net-2.2.1/src/pygpt_net/controller/dialogs/__init__.py
--rwxr-xr-x   0        0        0    12973 2024-04-27 07:58:32.750704 pygpt_net-2.2.1/src/pygpt_net/controller/dialogs/confirm.py
--rw-r--r--   0        0        0     5634 2024-03-07 01:04:26.437955 pygpt_net-2.2.1/src/pygpt_net/controller/dialogs/debug.py
--rwxr-xr-x   0        0        0     2582 2024-04-19 00:32:20.498428 pygpt_net-2.2.1/src/pygpt_net/controller/dialogs/info.py
--rwxr-xr-x   0        0        0    15576 2024-03-26 17:12:51.286309 pygpt_net-2.2.1/src/pygpt_net/controller/files.py
--rwxr-xr-x   0        0        0     4874 2024-04-21 01:33:54.239765 pygpt_net-2.2.1/src/pygpt_net/controller/finder.py
--rwxr-xr-x   0        0        0     7017 2024-04-27 14:05:11.727541 pygpt_net-2.2.1/src/pygpt_net/controller/idx/__init__.py
--rw-r--r--   0        0        0     2605 2024-02-29 03:07:51.274132 pygpt_net-2.2.1/src/pygpt_net/controller/idx/common.py
--rwxr-xr-x   0        0        0    21150 2024-04-17 04:14:11.980074 pygpt_net-2.2.1/src/pygpt_net/controller/idx/indexer.py
--rw-r--r--   0        0        0     7789 2024-03-03 03:52:54.350656 pygpt_net-2.2.1/src/pygpt_net/controller/idx/settings.py
--rw-r--r--   0        0        0     3186 2024-04-11 16:41:32.664297 pygpt_net-2.2.1/src/pygpt_net/controller/lang/__init__.py
--rw-r--r--   0        0        0     5080 2024-04-27 14:05:11.727541 pygpt_net-2.2.1/src/pygpt_net/controller/lang/custom.py
--rw-r--r--   0        0        0    19922 2024-04-27 14:05:11.727541 pygpt_net-2.2.1/src/pygpt_net/controller/lang/mapping.py
--rw-r--r--   0        0        0     3879 2024-01-15 13:47:55.919633 pygpt_net-2.2.1/src/pygpt_net/controller/lang/plugins.py
--rw-r--r--   0        0        0     2634 2024-01-22 12:10:21.917245 pygpt_net-2.2.1/src/pygpt_net/controller/lang/settings.py
--rwxr-xr-x   0        0        0     1566 2024-01-04 07:51:17.999390 pygpt_net-2.2.1/src/pygpt_net/controller/launcher.py
--rwxr-xr-x   0        0        0    11220 2024-04-21 01:33:54.243764 pygpt_net-2.2.1/src/pygpt_net/controller/layout.py
--rw-r--r--   0        0        0     6470 2024-03-15 15:31:21.786121 pygpt_net-2.2.1/src/pygpt_net/controller/mode.py
--rw-r--r--   0        0        0     4656 2024-01-30 20:56:32.772879 pygpt_net-2.2.1/src/pygpt_net/controller/model/__init__.py
--rw-r--r--   0        0        0    12599 2024-02-22 03:36:30.096422 pygpt_net-2.2.1/src/pygpt_net/controller/model/editor.py
--rwxr-xr-x   0        0        0    11579 2024-04-11 03:43:59.058733 pygpt_net-2.2.1/src/pygpt_net/controller/notepad.py
--rw-r--r--   0        0        0     2499 2024-04-10 01:07:30.184635 pygpt_net-2.2.1/src/pygpt_net/controller/painter/__init__.py
--rw-r--r--   0        0        0     4461 2024-01-23 23:46:30.495197 pygpt_net-2.2.1/src/pygpt_net/controller/painter/capture.py
--rw-r--r--   0        0        0     6292 2024-02-17 21:22:47.341663 pygpt_net-2.2.1/src/pygpt_net/controller/painter/common.py
--rw-r--r--   0        0        0    14032 2024-03-26 17:12:51.286309 pygpt_net-2.2.1/src/pygpt_net/controller/plugins/__init__.py
--rw-r--r--   0        0        0    11914 2024-03-07 01:04:26.441956 pygpt_net-2.2.1/src/pygpt_net/controller/plugins/presets.py
--rw-r--r--   0        0        0     6040 2024-04-10 03:33:51.491189 pygpt_net-2.2.1/src/pygpt_net/controller/plugins/settings.py
--rwxr-xr-x   0        0        0    15779 2024-04-22 22:35:26.796424 pygpt_net-2.2.1/src/pygpt_net/controller/presets/__init__.py
--rwxr-xr-x   0        0        0    14997 2024-04-22 22:35:26.800429 pygpt_net-2.2.1/src/pygpt_net/controller/presets/editor.py
--rw-r--r--   0        0        0     7562 2024-04-10 01:07:30.184635 pygpt_net-2.2.1/src/pygpt_net/controller/settings/__init__.py
--rwxr-xr-x   0        0        0    14833 2024-04-24 02:39:32.054775 pygpt_net-2.2.1/src/pygpt_net/controller/settings/editor.py
--rw-r--r--   0        0        0    20893 2024-04-19 00:32:20.498428 pygpt_net-2.2.1/src/pygpt_net/controller/settings/profile.py
--rwxr-xr-x   0        0        0     8597 2024-04-14 16:40:07.849541 pygpt_net-2.2.1/src/pygpt_net/controller/settings/workdir.py
--rwxr-xr-x   0        0        0     5988 2024-04-24 23:37:32.612565 pygpt_net-2.2.1/src/pygpt_net/controller/theme/__init__.py
--rwxr-xr-x   0        0        0     5435 2024-04-11 16:41:32.664297 pygpt_net-2.2.1/src/pygpt_net/controller/theme/common.py
--rw-r--r--   0        0        0     5085 2024-04-24 23:37:32.612565 pygpt_net-2.2.1/src/pygpt_net/controller/theme/markdown.py
--rw-r--r--   0        0        0     4631 2024-04-24 02:39:32.054775 pygpt_net-2.2.1/src/pygpt_net/controller/theme/menu.py
--rw-r--r--   0        0        0     5028 2024-04-24 23:37:32.612565 pygpt_net-2.2.1/src/pygpt_net/controller/theme/nodes.py
--rw-r--r--   0        0        0     6093 2024-04-11 03:43:59.058733 pygpt_net-2.2.1/src/pygpt_net/controller/ui/__init__.py
--rw-r--r--   0        0        0     4980 2024-04-27 14:05:11.727541 pygpt_net-2.2.1/src/pygpt_net/controller/ui/mode.py
--rw-r--r--   0        0        0     1902 2024-01-23 23:46:30.499197 pygpt_net-2.2.1/src/pygpt_net/controller/ui/vision.py
--rw-r--r--   0        0        0        0 2024-01-26 16:05:36.561120 pygpt_net-2.2.1/src/pygpt_net/core/__init__.py
--rw-r--r--   0        0        0     4330 2024-04-26 21:55:50.675598 pygpt_net-2.2.1/src/pygpt_net/core/assistants/__init__.py
--rw-r--r--   0        0        0     9275 2024-04-26 21:55:50.675598 pygpt_net-2.2.1/src/pygpt_net/core/assistants/files.py
--rw-r--r--   0        0        0     7998 2024-04-27 14:05:11.727541 pygpt_net-2.2.1/src/pygpt_net/core/assistants/store.py
--rwxr-xr-x   0        0        0    10240 2024-01-31 15:19:17.738030 pygpt_net-2.2.1/src/pygpt_net/core/attachments.py
--rw-r--r--   0        0        0     2708 2024-02-24 01:55:58.445111 pygpt_net-2.2.1/src/pygpt_net/core/audio.py
--rw-r--r--   0        0        0     4466 2024-03-15 15:31:21.786121 pygpt_net-2.2.1/src/pygpt_net/core/bridge.py
--rw-r--r--   0        0        0     6634 2024-03-12 06:49:17.164785 pygpt_net-2.2.1/src/pygpt_net/core/calendar/__init__.py
--rwxr-xr-x   0        0        0     4034 2024-02-21 16:18:39.952987 pygpt_net-2.2.1/src/pygpt_net/core/camera.py
--rw-r--r--   0        0        0     3130 2024-01-27 01:08:27.560991 pygpt_net-2.2.1/src/pygpt_net/core/chain/__init__.py
--rw-r--r--   0        0        0     4656 2024-01-27 01:08:27.560991 pygpt_net-2.2.1/src/pygpt_net/core/chain/chat.py
--rw-r--r--   0        0        0     5089 2024-01-27 01:08:27.560991 pygpt_net-2.2.1/src/pygpt_net/core/chain/completion.py
--rwxr-xr-x   0        0        0    10217 2024-03-17 14:26:02.923314 pygpt_net-2.2.1/src/pygpt_net/core/command.py
--rwxr-xr-x   0        0        0    31384 2024-04-17 06:16:54.016653 pygpt_net-2.2.1/src/pygpt_net/core/ctx/__init__.py
--rw-r--r--   0        0        0     7709 2024-02-27 05:21:39.767084 pygpt_net-2.2.1/src/pygpt_net/core/ctx/idx.py
--rw-r--r--   0        0        0    15726 2024-04-26 21:55:50.675598 pygpt_net-2.2.1/src/pygpt_net/core/db/__init__.py
--rw-r--r--   0        0        0     8884 2024-04-17 01:35:30.422055 pygpt_net-2.2.1/src/pygpt_net/core/db/viewer.py
--rwxr-xr-x   0        0        0     9240 2024-03-26 17:12:51.290309 pygpt_net-2.2.1/src/pygpt_net/core/debug/__init__.py
--rw-r--r--   0        0        0     1467 2024-02-25 18:06:16.205368 pygpt_net-2.2.1/src/pygpt_net/core/debug/agent.py
--rwxr-xr-x   0        0        0     2532 2024-04-26 21:55:50.675598 pygpt_net-2.2.1/src/pygpt_net/core/debug/assistants.py
--rwxr-xr-x   0        0        0     1626 2024-02-25 22:01:41.690831 pygpt_net-2.2.1/src/pygpt_net/core/debug/attachments.py
--rwxr-xr-x   0        0        0     2305 2024-04-10 01:07:30.184635 pygpt_net-2.2.1/src/pygpt_net/core/debug/config.py
--rwxr-xr-x   0        0        0     3543 2024-04-14 04:42:08.288289 pygpt_net-2.2.1/src/pygpt_net/core/debug/context.py
--rw-r--r--   0        0        0      776 2024-03-07 01:04:26.441956 pygpt_net-2.2.1/src/pygpt_net/core/debug/db.py
--rw-r--r--   0        0        0     5194 2024-03-12 06:49:17.164785 pygpt_net-2.2.1/src/pygpt_net/core/debug/indexes.py
--rwxr-xr-x   0        0        0     1848 2024-02-25 22:01:41.690831 pygpt_net-2.2.1/src/pygpt_net/core/debug/models.py
--rwxr-xr-x   0        0        0     1258 2024-02-25 22:01:41.690831 pygpt_net-2.2.1/src/pygpt_net/core/debug/plugins.py
--rwxr-xr-x   0        0        0     1994 2024-02-25 22:01:41.690831 pygpt_net-2.2.1/src/pygpt_net/core/debug/presets.py
--rwxr-xr-x   0        0        0     2666 2024-02-25 22:01:41.690831 pygpt_net-2.2.1/src/pygpt_net/core/debug/ui.py
--rwxr-xr-x   0        0        0     9012 2024-03-26 17:12:51.290309 pygpt_net-2.2.1/src/pygpt_net/core/dispatcher.py
--rwxr-xr-x   0        0        0    14537 2024-04-21 01:33:54.243764 pygpt_net-2.2.1/src/pygpt_net/core/filesystem/__init__.py
--rw-r--r--   0        0        0     4074 2024-03-26 17:12:51.290309 pygpt_net-2.2.1/src/pygpt_net/core/filesystem/actions.py
--rw-r--r--   0        0        0     4123 2024-04-22 03:13:23.727782 pygpt_net-2.2.1/src/pygpt_net/core/filesystem/editor.py
--rw-r--r--   0        0        0     3385 2024-03-19 09:04:41.050928 pygpt_net-2.2.1/src/pygpt_net/core/filesystem/types.py
--rw-r--r--   0        0        0     2753 2024-04-21 01:33:54.243764 pygpt_net-2.2.1/src/pygpt_net/core/filesystem/url.py
--rwxr-xr-x   0        0        0     3092 2024-01-23 23:46:30.499197 pygpt_net-2.2.1/src/pygpt_net/core/history.py
--rwxr-xr-x   0        0        0    17238 2024-04-17 01:35:30.422055 pygpt_net-2.2.1/src/pygpt_net/core/idx/__init__.py
--rwxr-xr-x   0        0        0    12300 2024-04-17 01:35:30.422055 pygpt_net-2.2.1/src/pygpt_net/core/idx/chat.py
--rw-r--r--   0        0        0     2226 2024-02-28 03:58:59.309445 pygpt_net-2.2.1/src/pygpt_net/core/idx/context.py
--rwxr-xr-x   0        0        0    31850 2024-04-17 01:35:30.422055 pygpt_net-2.2.1/src/pygpt_net/core/idx/indexing.py
--rw-r--r--   0        0        0     4016 2024-04-26 23:49:43.379197 pygpt_net-2.2.1/src/pygpt_net/core/idx/llm.py
--rw-r--r--   0        0        0     5304 2024-04-17 01:35:30.422055 pygpt_net-2.2.1/src/pygpt_net/core/idx/metadata.py
--rw-r--r--   0        0        0        0 2024-02-27 05:21:39.767084 pygpt_net-2.2.1/src/pygpt_net/core/idx/types/__init__.py
--rw-r--r--   0        0        0     3113 2024-02-27 05:21:39.767084 pygpt_net-2.2.1/src/pygpt_net/core/idx/types/ctx.py
--rw-r--r--   0        0        0     4722 2024-02-27 05:21:39.767084 pygpt_net-2.2.1/src/pygpt_net/core/idx/types/external.py
--rw-r--r--   0        0        0     3733 2024-02-27 05:21:39.771084 pygpt_net-2.2.1/src/pygpt_net/core/idx/types/files.py
--rwxr-xr-x   0        0        0     3774 2024-04-17 04:14:11.980074 pygpt_net-2.2.1/src/pygpt_net/core/idx/worker.py
--rwxr-xr-x   0        0        0     3288 2024-03-17 13:18:45.634349 pygpt_net-2.2.1/src/pygpt_net/core/image.py
--rwxr-xr-x   0        0        0      829 2023-12-31 03:18:56.426282 pygpt_net-2.2.1/src/pygpt_net/core/info.py
--rw-r--r--   0        0        0     2040 2024-03-25 10:26:39.426403 pygpt_net-2.2.1/src/pygpt_net/core/installer.py
--rw-r--r--   0        0        0     1168 2024-01-14 15:51:20.622630 pygpt_net-2.2.1/src/pygpt_net/core/llm/__init__.py
--rwxr-xr-x   0        0        0     5112 2024-04-11 16:41:32.664297 pygpt_net-2.2.1/src/pygpt_net/core/locale.py
--rw-r--r--   0        0        0     7573 2024-01-27 21:42:30.960980 pygpt_net-2.2.1/src/pygpt_net/core/models.py
--rw-r--r--   0        0        0     1913 2024-01-23 23:46:30.499197 pygpt_net-2.2.1/src/pygpt_net/core/modes.py
--rwxr-xr-x   0        0        0     3378 2024-04-10 01:07:30.184635 pygpt_net-2.2.1/src/pygpt_net/core/notepad.py
--rwxr-xr-x   0        0        0     4395 2024-03-09 21:41:28.185853 pygpt_net-2.2.1/src/pygpt_net/core/platforms.py
--rwxr-xr-x   0        0        0    14828 2024-04-28 08:05:35.578680 pygpt_net-2.2.1/src/pygpt_net/core/plugins.py
--rw-r--r--   0        0        0     9279 2024-03-17 13:18:45.634349 pygpt_net-2.2.1/src/pygpt_net/core/presets.py
--rw-r--r--   0        0        0     7650 2024-04-10 01:07:30.184635 pygpt_net-2.2.1/src/pygpt_net/core/profile.py
--rw-r--r--   0        0        0     2427 2024-04-22 22:35:26.800429 pygpt_net-2.2.1/src/pygpt_net/core/prompt/__init__.py
--rw-r--r--   0        0        0     2798 2024-04-22 22:35:26.800429 pygpt_net-2.2.1/src/pygpt_net/core/prompt/template.py
--rw-r--r--   0        0        0      489 2024-01-05 12:12:41.797675 pygpt_net-2.2.1/src/pygpt_net/core/render/__init__.py
--rw-r--r--   0        0        0     5024 2024-04-24 23:37:32.612565 pygpt_net-2.2.1/src/pygpt_net/core/render/base.py
--rwxr-xr-x   0        0        0      489 2024-04-21 01:33:54.243764 pygpt_net-2.2.1/src/pygpt_net/core/render/markdown/__init__.py
--rwxr-xr-x   0        0        0     5450 2024-04-22 05:35:04.663179 pygpt_net-2.2.1/src/pygpt_net/core/render/markdown/parser.py
--rwxr-xr-x   0        0        0    23291 2024-04-24 23:37:32.612565 pygpt_net-2.2.1/src/pygpt_net/core/render/markdown/renderer.py
--rw-r--r--   0        0        0      489 2024-01-05 13:07:04.262555 pygpt_net-2.2.1/src/pygpt_net/core/render/plain/__init__.py
--rw-r--r--   0        0        0    15716 2024-04-21 01:33:54.243764 pygpt_net-2.2.1/src/pygpt_net/core/render/plain/renderer.py
--rwxr-xr-x   0        0        0      489 2024-04-21 01:33:54.000000 pygpt_net-2.2.1/src/pygpt_net/core/render/web/__init__.py
--rwxr-xr-x   0        0        0     8564 2024-04-28 06:16:26.324027 pygpt_net-2.2.1/src/pygpt_net/core/render/web/parser.py
--rwxr-xr-x   0        0        0    42149 2024-04-25 03:37:50.192528 pygpt_net-2.2.1/src/pygpt_net/core/render/web/renderer.py
--rwxr-xr-x   0        0        0     7512 2024-04-24 23:37:32.612565 pygpt_net-2.2.1/src/pygpt_net/core/settings.py
--rw-r--r--   0        0        0        0 2024-04-21 01:33:54.243764 pygpt_net-2.2.1/src/pygpt_net/core/text/__init__.py
--rwxr-xr-x   0        0        0     6566 2024-04-21 01:33:54.243764 pygpt_net-2.2.1/src/pygpt_net/core/text/finder.py
--rw-r--r--   0        0        0     1970 2024-04-23 23:11:13.256158 pygpt_net-2.2.1/src/pygpt_net/core/text/utils.py
--rw-r--r--   0        0        0     6487 2024-04-21 01:33:54.243764 pygpt_net-2.2.1/src/pygpt_net/core/text/web_finder.py
--rwxr-xr-x   0        0        0    14040 2024-02-25 18:06:16.205368 pygpt_net-2.2.1/src/pygpt_net/core/tokens.py
--rw-r--r--   0        0        0    13722 2024-02-21 19:09:37.240983 pygpt_net-2.2.1/src/pygpt_net/core/updater/__init__.py
--rw-r--r--   0        0        0     2343 2024-02-24 01:55:58.445111 pygpt_net-2.2.1/src/pygpt_net/core/web.py
--rw-r--r--   0        0        0      901 2024-01-25 22:43:11.543975 pygpt_net-2.2.1/src/pygpt_net/core/worker.py
--rwxr-xr-x   0        0        0    10587 2024-04-28 08:05:35.578680 pygpt_net-2.2.1/src/pygpt_net/data/config/config.json
--rwxr-xr-x   0        0        0    18526 2024-04-28 08:05:35.578680 pygpt_net-2.2.1/src/pygpt_net/data/config/models.json
--rw-r--r--   0        0        0     1440 2024-04-28 08:05:35.578680 pygpt_net-2.2.1/src/pygpt_net/data/config/modes.json
--rwxr-xr-x   0        0        0      459 2024-01-13 13:04:53.113674 pygpt_net-2.2.1/src/pygpt_net/data/config/presets/batman_and_joker.json
--rw-r--r--   0        0        0     2702 2024-01-30 17:23:19.885579 pygpt_net-2.2.1/src/pygpt_net/data/config/presets/current.agent.json
--rwxr-xr-x   0        0        0      368 2024-01-30 17:23:19.885579 pygpt_net-2.2.1/src/pygpt_net/data/config/presets/current.assistant.json
--rwxr-xr-x   0        0        0      396 2024-01-30 17:23:19.885579 pygpt_net-2.2.1/src/pygpt_net/data/config/presets/current.chat.json
--rwxr-xr-x   0        0        0      385 2024-01-30 17:23:19.885579 pygpt_net-2.2.1/src/pygpt_net/data/config/presets/current.completion.json
--rwxr-xr-x   0        0        0      368 2024-01-30 17:23:19.885579 pygpt_net-2.2.1/src/pygpt_net/data/config/presets/current.img.json
--rwxr-xr-x   0        0        0      382 2024-01-30 17:23:19.885579 pygpt_net-2.2.1/src/pygpt_net/data/config/presets/current.langchain.json
--rw-r--r--   0        0        0      368 2024-03-03 02:59:46.037803 pygpt_net-2.2.1/src/pygpt_net/data/config/presets/current.llama_index.json
--rwxr-xr-x   0        0        0      392 2024-03-03 03:52:54.350656 pygpt_net-2.2.1/src/pygpt_net/data/config/presets/current.vision.json
--rwxr-xr-x   0        0        0      501 2024-01-30 17:23:19.885579 pygpt_net-2.2.1/src/pygpt_net/data/config/presets/dalle_white_cat.json
--rwxr-xr-x   0        0        0    32203 2024-04-21 01:33:54.243764 pygpt_net-2.2.1/src/pygpt_net/data/config/settings.json
--rw-r--r--   0        0        0      804 2024-03-17 13:18:45.634349 pygpt_net-2.2.1/src/pygpt_net/data/config/settings_section.json
--rwxr-xr-x   0        0        0      664 2024-03-18 04:54:07.000000 pygpt_net-2.2.1/src/pygpt_net/data/css/fix_windows.css
--rwxr-xr-x   0        0        0     1122 2024-04-19 00:29:50.000000 pygpt_net-2.2.1/src/pygpt_net/data/css/markdown.css
--rwxr-xr-x   0        0        0      730 2024-04-19 00:29:50.000000 pygpt_net-2.2.1/src/pygpt_net/data/css/markdown.dark.css
--rwxr-xr-x   0        0        0      833 2024-04-19 00:29:50.000000 pygpt_net-2.2.1/src/pygpt_net/data/css/markdown.light.css
--rwxr-xr-x   0        0        0      400 2024-04-20 05:54:38.000000 pygpt_net-2.2.1/src/pygpt_net/data/css/style.css
--rwxr-xr-x   0        0        0      729 2024-04-21 01:33:54.243764 pygpt_net-2.2.1/src/pygpt_net/data/css/style.dark.css
--rwxr-xr-x   0        0        0     1726 2024-04-20 05:55:02.000000 pygpt_net-2.2.1/src/pygpt_net/data/css/style.light.css
--rwxr-xr-x   0        0        0     3407 2024-04-24 23:37:32.612565 pygpt_net-2.2.1/src/pygpt_net/data/css/web.css
--rwxr-xr-x   0        0        0     1260 2024-04-25 03:37:50.192528 pygpt_net-2.2.1/src/pygpt_net/data/css/web.dark.css
--rwxr-xr-x   0        0        0     1235 2024-04-25 03:07:07.934949 pygpt_net-2.2.1/src/pygpt_net/data/css/web.light.css
--rwxr-xr-x   0        0        0    69484 2023-12-08 15:03:16.000000 pygpt_net-2.2.1/src/pygpt_net/data/fonts/Lato/Lato-Black.ttf
--rwxr-xr-x   0        0        0    71948 2023-12-08 15:03:16.000000 pygpt_net-2.2.1/src/pygpt_net/data/fonts/Lato/Lato-BlackItalic.ttf
--rwxr-xr-x   0        0        0    73316 2023-12-08 15:03:16.000000 pygpt_net-2.2.1/src/pygpt_net/data/fonts/Lato/Lato-Bold.ttf
--rwxr-xr-x   0        0        0    77680 2023-12-08 15:03:16.000000 pygpt_net-2.2.1/src/pygpt_net/data/fonts/Lato/Lato-BoldItalic.ttf
--rwxr-xr-x   0        0        0    75744 2023-12-08 15:03:16.000000 pygpt_net-2.2.1/src/pygpt_net/data/fonts/Lato/Lato-Italic.ttf
--rwxr-xr-x   0        0        0    77192 2023-12-08 15:03:16.000000 pygpt_net-2.2.1/src/pygpt_net/data/fonts/Lato/Lato-Light.ttf
--rwxr-xr-x   0        0        0    49064 2023-12-08 15:03:16.000000 pygpt_net-2.2.1/src/pygpt_net/data/fonts/Lato/Lato-LightItalic.ttf
--rwxr-xr-x   0        0        0    75136 2023-12-08 15:03:16.000000 pygpt_net-2.2.1/src/pygpt_net/data/fonts/Lato/Lato-Regular.ttf
--rwxr-xr-x   0        0        0    69968 2023-12-08 15:03:16.000000 pygpt_net-2.2.1/src/pygpt_net/data/fonts/Lato/Lato-Thin.ttf
--rwxr-xr-x   0        0        0    48848 2023-12-08 15:03:16.000000 pygpt_net-2.2.1/src/pygpt_net/data/fonts/Lato/Lato-ThinItalic.ttf
--rwxr-xr-x   0        0        0     4500 2023-12-08 15:03:16.000000 pygpt_net-2.2.1/src/pygpt_net/data/fonts/Lato/OFL.txt
--rw-r--r--   0        0        0    77432 2024-04-08 04:19:15.417912 pygpt_net-2.2.1/src/pygpt_net/data/fonts/MonaspaceArgon/MonaspaceArgon-Bold.otf
--rw-r--r--   0        0        0    82112 2024-04-08 04:19:15.417912 pygpt_net-2.2.1/src/pygpt_net/data/fonts/MonaspaceArgon/MonaspaceArgon-BoldItalic.otf
--rw-r--r--   0        0        0    81240 2024-04-08 04:19:15.417912 pygpt_net-2.2.1/src/pygpt_net/data/fonts/MonaspaceArgon/MonaspaceArgon-Italic.otf
--rw-r--r--   0        0        0    75476 2024-04-08 04:19:15.421912 pygpt_net-2.2.1/src/pygpt_net/data/fonts/MonaspaceArgon/MonaspaceArgon-Regular.otf
--rw-r--r--   0        0        0    75000 2024-04-08 04:19:15.421912 pygpt_net-2.2.1/src/pygpt_net/data/fonts/MonaspaceKrypton/MonaspaceKrypton-Bold.otf
--rw-r--r--   0        0        0    77804 2024-04-08 04:19:15.421912 pygpt_net-2.2.1/src/pygpt_net/data/fonts/MonaspaceKrypton/MonaspaceKrypton-BoldItalic.otf
--rw-r--r--   0        0        0    76752 2024-04-08 04:19:15.421912 pygpt_net-2.2.1/src/pygpt_net/data/fonts/MonaspaceKrypton/MonaspaceKrypton-Italic.otf
--rw-r--r--   0        0        0    74248 2024-04-08 04:19:15.421912 pygpt_net-2.2.1/src/pygpt_net/data/fonts/MonaspaceKrypton/MonaspaceKrypton-Regular.otf
--rw-r--r--   0        0        0    74120 2024-04-08 04:19:15.421912 pygpt_net-2.2.1/src/pygpt_net/data/fonts/MonaspaceNeon/MonaspaceNeon-Bold.otf
--rw-r--r--   0        0        0    79236 2024-04-08 04:19:15.421912 pygpt_net-2.2.1/src/pygpt_net/data/fonts/MonaspaceNeon/MonaspaceNeon-BoldItalic.otf
--rw-r--r--   0        0        0    78488 2024-04-08 04:19:15.425912 pygpt_net-2.2.1/src/pygpt_net/data/fonts/MonaspaceNeon/MonaspaceNeon-Italic.otf
--rw-r--r--   0        0        0    73232 2024-04-08 04:19:15.425912 pygpt_net-2.2.1/src/pygpt_net/data/fonts/MonaspaceNeon/MonaspaceNeon-Regular.otf
--rw-r--r--   0        0        0    88992 2024-04-08 04:19:15.425912 pygpt_net-2.2.1/src/pygpt_net/data/fonts/MonaspaceRadon/MonaspaceRadon-Bold.otf
--rw-r--r--   0        0        0    94348 2024-04-08 04:19:15.425912 pygpt_net-2.2.1/src/pygpt_net/data/fonts/MonaspaceRadon/MonaspaceRadon-BoldItalic.otf
--rw-r--r--   0        0        0    93720 2024-04-08 04:19:15.425912 pygpt_net-2.2.1/src/pygpt_net/data/fonts/MonaspaceRadon/MonaspaceRadon-Italic.otf
--rw-r--r--   0        0        0    88668 2024-04-08 04:19:15.429912 pygpt_net-2.2.1/src/pygpt_net/data/fonts/MonaspaceRadon/MonaspaceRadon-Regular.otf
--rw-r--r--   0        0        0    79280 2024-04-08 04:19:15.429912 pygpt_net-2.2.1/src/pygpt_net/data/fonts/MonaspaceXenon/MonaspaceXenon-Bold.otf
--rw-r--r--   0        0        0    85648 2024-04-08 04:19:15.429912 pygpt_net-2.2.1/src/pygpt_net/data/fonts/MonaspaceXenon/MonaspaceXenon-BoldItalic.otf
--rw-r--r--   0        0        0    85824 2024-04-08 04:19:15.429912 pygpt_net-2.2.1/src/pygpt_net/data/fonts/MonaspaceXenon/MonaspaceXenon-Italic.otf
--rw-r--r--   0        0        0    80200 2024-04-08 04:19:15.429912 pygpt_net-2.2.1/src/pygpt_net/data/fonts/MonaspaceXenon/MonaspaceXenon-Regular.otf
--rwxr-xr-x   0        0        0     4352 2024-03-18 04:54:07.633826 pygpt_net-2.2.1/src/pygpt_net/data/fonts/SpaceMono/OFL.txt
--rwxr-xr-x   0        0        0    86636 2024-03-18 04:54:07.633826 pygpt_net-2.2.1/src/pygpt_net/data/fonts/SpaceMono/SpaceMono-Bold.ttf
--rwxr-xr-x   0        0        0    95292 2024-03-18 04:54:07.633826 pygpt_net-2.2.1/src/pygpt_net/data/fonts/SpaceMono/SpaceMono-BoldItalic.ttf
--rwxr-xr-x   0        0        0   103524 2024-03-18 04:54:07.633826 pygpt_net-2.2.1/src/pygpt_net/data/fonts/SpaceMono/SpaceMono-Italic.ttf
--rwxr-xr-x   0        0        0    90904 2024-03-18 04:54:07.637826 pygpt_net-2.2.1/src/pygpt_net/data/fonts/SpaceMono/SpaceMono-Regular.ttf
--rwxr-xr-x   0        0        0     3461 2023-04-14 00:10:28.000000 pygpt_net-2.2.1/src/pygpt_net/data/icon.ico
--rwxr-xr-x   0        0        0    13970 2023-04-14 00:10:28.000000 pygpt_net-2.2.1/src/pygpt_net/data/icon.png
--rw-r--r--   0        0        0     5471 2024-01-29 18:11:38.035830 pygpt_net-2.2.1/src/pygpt_net/data/icon_tray_busy.ico
--rw-r--r--   0        0        0    14837 2024-01-29 18:11:38.035830 pygpt_net-2.2.1/src/pygpt_net/data/icon_tray_error.ico
--rw-r--r--   0        0        0     4209 2024-01-29 18:11:38.035830 pygpt_net-2.2.1/src/pygpt_net/data/icon_tray_idle.ico
--rw-r--r--   0        0        0      538 2024-01-30 17:23:19.885579 pygpt_net-2.2.1/src/pygpt_net/data/icons/abc.svg
--rw-r--r--   0        0        0      178 2024-01-30 17:23:19.885579 pygpt_net-2.2.1/src/pygpt_net/data/icons/add.svg
--rw-r--r--   0        0        0      463 2024-01-30 17:23:19.885579 pygpt_net-2.2.1/src/pygpt_net/data/icons/add_circle.svg
--rw-r--r--   0        0        0      348 2024-01-30 17:23:19.885579 pygpt_net-2.2.1/src/pygpt_net/data/icons/add_folder.svg
--rw-r--r--   0        0        0      391 2024-01-30 17:23:19.885579 pygpt_net-2.2.1/src/pygpt_net/data/icons/add_library.svg
--rw-r--r--   0        0        0      558 2024-01-30 17:23:19.885579 pygpt_net-2.2.1/src/pygpt_net/data/icons/alarm.svg
--rw-r--r--   0        0        0     1027 2024-01-30 17:23:19.885579 pygpt_net-2.2.1/src/pygpt_net/data/icons/apps.svg
--rw-r--r--   0        0        0      267 2024-01-30 17:23:19.885579 pygpt_net-2.2.1/src/pygpt_net/data/icons/asterisk.svg
--rw-r--r--   0        0        0      429 2024-01-30 17:23:19.885579 pygpt_net-2.2.1/src/pygpt_net/data/icons/attachment.svg
--rw-r--r--   0        0        0      422 2024-01-30 17:23:19.885579 pygpt_net-2.2.1/src/pygpt_net/data/icons/attachments.svg
--rw-r--r--   0        0        0      185 2024-01-30 17:23:19.885579 pygpt_net-2.2.1/src/pygpt_net/data/icons/back.svg
--rw-r--r--   0        0        0      395 2024-01-30 17:23:19.885579 pygpt_net-2.2.1/src/pygpt_net/data/icons/backspace.svg
--rw-r--r--   0        0        0      472 2024-01-30 17:23:19.885579 pygpt_net-2.2.1/src/pygpt_net/data/icons/block.svg
--rw-r--r--   0        0        0      255 2024-01-30 17:23:19.885579 pygpt_net-2.2.1/src/pygpt_net/data/icons/bookmark.svg
--rw-r--r--   0        0        0      423 2024-01-30 17:23:19.885579 pygpt_net-2.2.1/src/pygpt_net/data/icons/brush.svg
--rw-r--r--   0        0        0      523 2024-01-30 17:23:19.885579 pygpt_net-2.2.1/src/pygpt_net/data/icons/build.svg
--rw-r--r--   0        0        0      927 2024-01-30 17:23:19.885579 pygpt_net-2.2.1/src/pygpt_net/data/icons/calendar.svg
--rw-r--r--   0        0        0      496 2024-01-30 17:23:19.885579 pygpt_net-2.2.1/src/pygpt_net/data/icons/camera.svg
--rw-r--r--   0        0        0      987 2024-03-09 21:41:28.185853 pygpt_net-2.2.1/src/pygpt_net/data/icons/chat/audio.png
--rw-r--r--   0        0        0      798 2024-03-09 21:41:28.185853 pygpt_net-2.2.1/src/pygpt_net/data/icons/chat/copy.png
--rw-r--r--   0        0        0      737 2024-03-09 21:41:28.185853 pygpt_net-2.2.1/src/pygpt_net/data/icons/chat/delete.png
--rw-r--r--   0        0        0      837 2024-03-09 21:41:28.185853 pygpt_net-2.2.1/src/pygpt_net/data/icons/chat/edit.png
--rw-r--r--   0        0        0      715 2024-03-10 08:19:22.357281 pygpt_net-2.2.1/src/pygpt_net/data/icons/chat/join.png
--rw-r--r--   0        0        0      956 2024-03-09 21:41:28.185853 pygpt_net-2.2.1/src/pygpt_net/data/icons/chat/reload.png
--rw-r--r--   0        0        0      336 2024-01-30 17:23:19.885579 pygpt_net-2.2.1/src/pygpt_net/data/icons/chat.svg
--rw-r--r--   0        0        0      174 2024-01-30 17:23:19.885579 pygpt_net-2.2.1/src/pygpt_net/data/icons/check.svg
--rw-r--r--   0        0        0      459 2024-01-30 17:23:19.885579 pygpt_net-2.2.1/src/pygpt_net/data/icons/check_circle.svg
--rw-r--r--   0        0        0      265 2024-01-30 17:23:19.885579 pygpt_net-2.2.1/src/pygpt_net/data/icons/checklist.svg
--rw-r--r--   0        0        0      406 2024-01-30 17:23:19.885579 pygpt_net-2.2.1/src/pygpt_net/data/icons/circle.svg
--rw-r--r--   0        0        0      191 2024-01-30 17:23:19.885579 pygpt_net-2.2.1/src/pygpt_net/data/icons/clear.svg
--rw-r--r--   0        0        0      411 2024-01-30 17:23:19.885579 pygpt_net-2.2.1/src/pygpt_net/data/icons/clock.svg
--rw-r--r--   0        0        0      218 2024-01-30 17:23:19.885579 pygpt_net-2.2.1/src/pygpt_net/data/icons/close.svg
--rw-r--r--   0        0        0      503 2024-01-30 17:23:19.885579 pygpt_net-2.2.1/src/pygpt_net/data/icons/close_circle.svg
--rw-r--r--   0        0        0      224 2024-01-30 17:23:19.885579 pygpt_net-2.2.1/src/pygpt_net/data/icons/code.svg
--rw-r--r--   0        0        0      298 2024-01-30 17:23:19.885579 pygpt_net-2.2.1/src/pygpt_net/data/icons/computer.svg
--rw-r--r--   0        0        0      336 2024-01-30 17:23:19.885579 pygpt_net-2.2.1/src/pygpt_net/data/icons/copy.svg
--rw-r--r--   0        0        0      264 2024-01-30 17:23:19.885579 pygpt_net-2.2.1/src/pygpt_net/data/icons/crop.svg
--rw-r--r--   0        0        0      666 2024-01-30 17:23:19.885579 pygpt_net-2.2.1/src/pygpt_net/data/icons/cut.svg
--rw-r--r--   0        0        0      725 2024-01-30 17:23:19.885579 pygpt_net-2.2.1/src/pygpt_net/data/icons/db.svg
--rw-r--r--   0        0        0      271 2024-01-30 17:23:19.889579 pygpt_net-2.2.1/src/pygpt_net/data/icons/delete.svg
--rw-r--r--   0        0        0      174 2024-01-30 17:23:19.889579 pygpt_net-2.2.1/src/pygpt_net/data/icons/done.svg
--rw-r--r--   0        0        0      274 2024-01-30 17:23:19.889579 pygpt_net-2.2.1/src/pygpt_net/data/icons/download.svg
--rw-r--r--   0        0        0      283 2024-01-30 17:23:19.889579 pygpt_net-2.2.1/src/pygpt_net/data/icons/draft.svg
--rw-r--r--   0        0        0      323 2024-01-30 17:23:19.889579 pygpt_net-2.2.1/src/pygpt_net/data/icons/drag.svg
--rw-r--r--   0        0        0      325 2024-01-30 17:23:19.889579 pygpt_net-2.2.1/src/pygpt_net/data/icons/edit.svg
--rw-r--r--   0        0        0      497 2024-01-30 17:23:19.889579 pygpt_net-2.2.1/src/pygpt_net/data/icons/emergency.svg
--rw-r--r--   0        0        0      195 2024-01-30 17:23:19.889579 pygpt_net-2.2.1/src/pygpt_net/data/icons/equalizer.svg
--rw-r--r--   0        0        0      533 2024-01-30 17:23:19.889579 pygpt_net-2.2.1/src/pygpt_net/data/icons/error.svg
--rw-r--r--   0        0        0      372 2024-01-30 17:23:19.889579 pygpt_net-2.2.1/src/pygpt_net/data/icons/event_available.svg
--rw-r--r--   0        0        0      174 2024-01-30 17:23:19.889579 pygpt_net-2.2.1/src/pygpt_net/data/icons/expand.svg
--rw-r--r--   0        0        0      247 2024-01-30 17:23:19.889579 pygpt_net-2.2.1/src/pygpt_net/data/icons/fast_forward.svg
--rw-r--r--   0        0        0      250 2024-01-30 17:23:19.889579 pygpt_net-2.2.1/src/pygpt_net/data/icons/fast_rewind.svg
--rw-r--r--   0        0        0      504 2024-01-30 17:23:19.889579 pygpt_net-2.2.1/src/pygpt_net/data/icons/favorite.svg
--rw-r--r--   0        0        0      297 2024-01-30 17:23:19.889579 pygpt_net-2.2.1/src/pygpt_net/data/icons/folder.svg
--rw-r--r--   0        0        0      249 2024-01-30 17:23:19.889579 pygpt_net-2.2.1/src/pygpt_net/data/icons/folder_filled.svg
--rw-r--r--   0        0        0      186 2024-01-30 17:23:19.889579 pygpt_net-2.2.1/src/pygpt_net/data/icons/forward.svg
--rw-r--r--   0        0        0      194 2024-01-30 17:23:19.889579 pygpt_net-2.2.1/src/pygpt_net/data/icons/full.svg
--rw-r--r--   0        0        0      249 2024-01-30 17:23:19.889579 pygpt_net-2.2.1/src/pygpt_net/data/icons/fullscreen.svg
--rw-r--r--   0        0        0      459 2024-01-30 17:23:19.889579 pygpt_net-2.2.1/src/pygpt_net/data/icons/grid.svg
--rw-r--r--   0        0        0      602 2024-01-30 17:23:19.889579 pygpt_net-2.2.1/src/pygpt_net/data/icons/hearing.svg
--rw-r--r--   0        0        0      691 2024-01-30 17:23:19.889579 pygpt_net-2.2.1/src/pygpt_net/data/icons/help.svg
--rw-r--r--   0        0        0      440 2024-01-30 17:23:19.889579 pygpt_net-2.2.1/src/pygpt_net/data/icons/history.svg
--rw-r--r--   0        0        0      239 2024-01-30 17:23:19.889579 pygpt_net-2.2.1/src/pygpt_net/data/icons/home.svg
--rw-r--r--   0        0        0      176 2024-01-30 17:23:19.889579 pygpt_net-2.2.1/src/pygpt_net/data/icons/home_filled.svg
--rw-r--r--   0        0        0      323 2024-01-30 17:23:19.889579 pygpt_net-2.2.1/src/pygpt_net/data/icons/image.svg
--rw-r--r--   0        0        0      531 2024-01-30 17:23:19.889579 pygpt_net-2.2.1/src/pygpt_net/data/icons/info.svg
--rw-r--r--   0        0        0      337 2024-01-30 17:23:19.889579 pygpt_net-2.2.1/src/pygpt_net/data/icons/input.svg
--rw-r--r--   0        0        0      541 2024-01-30 17:23:19.889579 pygpt_net-2.2.1/src/pygpt_net/data/icons/key.svg
--rw-r--r--   0        0        0      517 2024-01-30 17:23:19.889579 pygpt_net-2.2.1/src/pygpt_net/data/icons/keyboard.svg
--rw-r--r--   0        0        0      972 2024-01-30 17:23:19.889579 pygpt_net-2.2.1/src/pygpt_net/data/icons/language.svg
--rw-r--r--   0        0        0      491 2024-01-30 17:23:19.889579 pygpt_net-2.2.1/src/pygpt_net/data/icons/list.svg
--rw-r--r--   0        0        0      495 2024-01-30 17:23:19.889579 pygpt_net-2.2.1/src/pygpt_net/data/icons/lock.svg
--rw-r--r--   0        0        0      273 2024-01-30 17:23:19.889579 pygpt_net-2.2.1/src/pygpt_net/data/icons/logout.svg
--rw-r--r--   0        0        0      392 2024-01-30 17:23:19.889579 pygpt_net-2.2.1/src/pygpt_net/data/icons/map.svg
--rw-r--r--   0        0        0      431 2024-01-30 17:23:19.889579 pygpt_net-2.2.1/src/pygpt_net/data/icons/memory.svg
--rw-r--r--   0        0        0      189 2024-01-30 17:23:19.889579 pygpt_net-2.2.1/src/pygpt_net/data/icons/menu.svg
--rw-r--r--   0        0        0      447 2024-01-30 17:23:19.889579 pygpt_net-2.2.1/src/pygpt_net/data/icons/mic.svg
--rw-r--r--   0        0        0      485 2024-01-30 17:23:19.889579 pygpt_net-2.2.1/src/pygpt_net/data/icons/mic_off.svg
--rw-r--r--   0        0        0      423 2024-01-30 17:23:19.889579 pygpt_net-2.2.1/src/pygpt_net/data/icons/more_horizontal.svg
--rw-r--r--   0        0        0      491 2024-01-30 17:23:19.889579 pygpt_net-2.2.1/src/pygpt_net/data/icons/mute.svg
--rw-r--r--   0        0        0      296 2024-01-30 17:23:19.889579 pygpt_net-2.2.1/src/pygpt_net/data/icons/open_tab.svg
--rw-r--r--   0        0        0      846 2024-01-30 17:23:19.889579 pygpt_net-2.2.1/src/pygpt_net/data/icons/palette.svg
--rw-r--r--   0        0        0      431 2024-01-30 17:23:19.889579 pygpt_net-2.2.1/src/pygpt_net/data/icons/paste.svg
--rw-r--r--   0        0        0      250 2024-01-30 17:23:19.889579 pygpt_net-2.2.1/src/pygpt_net/data/icons/pause.svg
--rw-r--r--   0        0        0      454 2024-01-30 17:23:19.889579 pygpt_net-2.2.1/src/pygpt_net/data/icons/pause_circle.svg
--rw-r--r--   0        0        0      377 2024-01-30 17:23:19.889579 pygpt_net-2.2.1/src/pygpt_net/data/icons/photos.svg
--rw-r--r--   0        0        0      441 2024-01-30 17:23:19.889579 pygpt_net-2.2.1/src/pygpt_net/data/icons/pin.svg
--rw-r--r--   0        0        0      186 2024-01-30 17:23:19.889579 pygpt_net-2.2.1/src/pygpt_net/data/icons/play.svg
--rw-r--r--   0        0        0      197 2024-01-30 17:23:19.889579 pygpt_net-2.2.1/src/pygpt_net/data/icons/play_pause.svg
--rw-r--r--   0        0        0      246 2024-01-30 17:23:19.889579 pygpt_net-2.2.1/src/pygpt_net/data/icons/playlist_add.svg
--rw-r--r--   0        0        0      318 2024-01-30 17:23:19.889579 pygpt_net-2.2.1/src/pygpt_net/data/icons/power.svg
--rw-r--r--   0        0        0      478 2024-01-30 17:23:19.889579 pygpt_net-2.2.1/src/pygpt_net/data/icons/print.svg
--rw-r--r--   0        0        0      598 2024-01-30 17:23:19.889579 pygpt_net-2.2.1/src/pygpt_net/data/icons/public_filled.svg
--rw-r--r--   0        0        0      283 2024-01-30 20:56:32.772879 pygpt_net-2.2.1/src/pygpt_net/data/icons/redo.svg
--rw-r--r--   0        0        0      329 2024-01-30 17:23:19.889579 pygpt_net-2.2.1/src/pygpt_net/data/icons/reload.svg
--rw-r--r--   0        0        0      260 2024-01-30 17:23:19.889579 pygpt_net-2.2.1/src/pygpt_net/data/icons/repeat.svg
--rw-r--r--   0        0        0      400 2024-01-30 17:23:19.889579 pygpt_net-2.2.1/src/pygpt_net/data/icons/replay.svg
--rw-r--r--   0        0        0      401 2024-01-30 17:23:19.889579 pygpt_net-2.2.1/src/pygpt_net/data/icons/resize.svg
--rw-r--r--   0        0        0      615 2024-01-30 17:23:19.889579 pygpt_net-2.2.1/src/pygpt_net/data/icons/robot.svg
--rw-r--r--   0        0        0      807 2024-01-30 17:23:19.889579 pygpt_net-2.2.1/src/pygpt_net/data/icons/router.svg
--rw-r--r--   0        0        0      384 2024-01-30 17:23:19.889579 pygpt_net-2.2.1/src/pygpt_net/data/icons/save.svg
--rw-r--r--   0        0        0      469 2024-01-30 17:23:19.889579 pygpt_net-2.2.1/src/pygpt_net/data/icons/schedule.svg
--rw-r--r--   0        0        0      396 2024-01-30 17:23:19.889579 pygpt_net-2.2.1/src/pygpt_net/data/icons/screenshot.svg
--rw-r--r--   0        0        0      372 2024-01-30 17:23:19.889579 pygpt_net-2.2.1/src/pygpt_net/data/icons/search.svg
--rw-r--r--   0        0        0      274 2024-01-30 17:23:19.889579 pygpt_net-2.2.1/src/pygpt_net/data/icons/security.svg
--rw-r--r--   0        0        0      660 2024-01-30 17:23:19.889579 pygpt_net-2.2.1/src/pygpt_net/data/icons/sensors.svg
--rw-r--r--   0        0        0      767 2024-01-30 17:23:19.889579 pygpt_net-2.2.1/src/pygpt_net/data/icons/settings.svg
--rw-r--r--   0        0        0      475 2024-01-30 17:23:19.889579 pygpt_net-2.2.1/src/pygpt_net/data/icons/settings_filled.svg
--rw-r--r--   0        0        0      792 2024-01-30 17:23:19.889579 pygpt_net-2.2.1/src/pygpt_net/data/icons/share.svg
--rw-r--r--   0        0        0      469 2024-01-30 17:23:19.889579 pygpt_net-2.2.1/src/pygpt_net/data/icons/shedule.svg
--rw-r--r--   0        0        0      189 2024-01-30 17:23:19.889579 pygpt_net-2.2.1/src/pygpt_net/data/icons/sort.svg
--rw-r--r--   0        0        0      386 2024-01-30 17:23:19.889579 pygpt_net-2.2.1/src/pygpt_net/data/icons/stack.svg
--rw-r--r--   0        0        0      306 2024-01-30 17:23:19.889579 pygpt_net-2.2.1/src/pygpt_net/data/icons/stacks.svg
--rw-r--r--   0        0        0      291 2024-01-30 17:23:19.889579 pygpt_net-2.2.1/src/pygpt_net/data/icons/star.svg
--rw-r--r--   0        0        0      188 2024-01-30 17:23:19.893578 pygpt_net-2.2.1/src/pygpt_net/data/icons/stop.svg
--rw-r--r--   0        0        0      432 2024-01-30 17:23:19.893578 pygpt_net-2.2.1/src/pygpt_net/data/icons/stop_circle.svg
--rw-r--r--   0        0        0      381 2024-01-30 17:23:19.893578 pygpt_net-2.2.1/src/pygpt_net/data/icons/sync.svg
--rw-r--r--   0        0        0      317 2024-01-30 17:23:19.893578 pygpt_net-2.2.1/src/pygpt_net/data/icons/tag.svg
--rw-r--r--   0        0        0      334 2024-01-30 17:23:19.893578 pygpt_net-2.2.1/src/pygpt_net/data/icons/task.svg
--rw-r--r--   0        0        0      336 2024-01-30 17:23:19.893578 pygpt_net-2.2.1/src/pygpt_net/data/icons/terminal.svg
--rw-r--r--   0        0        0      204 2024-01-30 17:23:19.893578 pygpt_net-2.2.1/src/pygpt_net/data/icons/text.svg
--rw-r--r--   0        0        0      329 2024-01-30 17:23:19.893578 pygpt_net-2.2.1/src/pygpt_net/data/icons/textfile.svg
--rw-r--r--   0        0        0      479 2024-01-30 17:23:19.893578 pygpt_net-2.2.1/src/pygpt_net/data/icons/timer.svg
--rw-r--r--   0        0        0      321 2024-01-30 17:23:19.893578 pygpt_net-2.2.1/src/pygpt_net/data/icons/today.svg
--rw-r--r--   0        0        0      308 2024-01-30 17:23:19.893578 pygpt_net-2.2.1/src/pygpt_net/data/icons/tune.svg
--rw-r--r--   0        0        0      282 2024-01-30 17:23:19.893578 pygpt_net-2.2.1/src/pygpt_net/data/icons/undo.svg
--rw-r--r--   0        0        0      444 2024-01-30 17:23:19.893578 pygpt_net-2.2.1/src/pygpt_net/data/icons/update.svg
--rw-r--r--   0        0        0      392 2024-01-30 17:23:19.893578 pygpt_net-2.2.1/src/pygpt_net/data/icons/updater.svg
--rw-r--r--   0        0        0      276 2024-01-30 17:23:19.893578 pygpt_net-2.2.1/src/pygpt_net/data/icons/upload.svg
--rw-r--r--   0        0        0      339 2024-01-30 17:23:19.893578 pygpt_net-2.2.1/src/pygpt_net/data/icons/video.svg
--rw-r--r--   0        0        0      550 2024-01-30 17:23:19.893578 pygpt_net-2.2.1/src/pygpt_net/data/icons/view.svg
--rw-r--r--   0        0        0      736 2024-01-30 17:23:19.893578 pygpt_net-2.2.1/src/pygpt_net/data/icons/voice.svg
--rw-r--r--   0        0        0      374 2024-01-30 17:23:19.893578 pygpt_net-2.2.1/src/pygpt_net/data/icons/volume.svg
--rw-r--r--   0        0        0      310 2024-01-30 17:23:19.893578 pygpt_net-2.2.1/src/pygpt_net/data/icons/warning.svg
--rw-r--r--   0        0        0      300 2024-01-30 17:23:19.893578 pygpt_net-2.2.1/src/pygpt_net/data/icons/webcam.svg
--rw-r--r--   0        0        0      375 2024-02-29 03:07:51.274132 pygpt_net-2.2.1/src/pygpt_net/data/icons/webcam_off.svg
--rw-r--r--   0        0        0      325 2024-01-30 17:23:19.893578 pygpt_net-2.2.1/src/pygpt_net/data/icons/width.svg
--rw-r--r--   0        0        0      336 2024-01-30 17:23:19.893578 pygpt_net-2.2.1/src/pygpt_net/data/icons/window.svg
--rw-r--r--   0        0        0      365 2024-01-30 17:23:19.893578 pygpt_net-2.2.1/src/pygpt_net/data/icons/work.svg
--rw-r--r--   0        0        0      422 2024-01-30 17:23:19.893578 pygpt_net-2.2.1/src/pygpt_net/data/icons/zoom_in.svg
--rw-r--r--   0        0        0      396 2024-01-30 17:23:19.893578 pygpt_net-2.2.1/src/pygpt_net/data/icons/zoom_out.svg
--rwxr-xr-x   0        0        0    45043 2024-04-26 21:55:50.675598 pygpt_net-2.2.1/src/pygpt_net/data/locale/locale.de.ini
--rwxr-xr-x   0        0        0    53434 2024-04-28 06:16:26.324027 pygpt_net-2.2.1/src/pygpt_net/data/locale/locale.en.ini
--rwxr-xr-x   0        0        0    45213 2024-04-26 21:55:50.675598 pygpt_net-2.2.1/src/pygpt_net/data/locale/locale.es.ini
--rwxr-xr-x   0        0        0    46829 2024-04-26 21:55:50.675598 pygpt_net-2.2.1/src/pygpt_net/data/locale/locale.fr.ini
--rwxr-xr-x   0        0        0    44302 2024-04-26 21:55:50.679597 pygpt_net-2.2.1/src/pygpt_net/data/locale/locale.it.ini
--rwxr-xr-x   0        0        0    44211 2024-04-26 21:55:50.679597 pygpt_net-2.2.1/src/pygpt_net/data/locale/locale.pl.ini
--rwxr-xr-x   0        0        0    62420 2024-04-26 21:55:50.679597 pygpt_net-2.2.1/src/pygpt_net/data/locale/locale.uk.ini
--rwxr-xr-x   0        0        0    48001 2024-04-26 21:55:50.679597 pygpt_net-2.2.1/src/pygpt_net/data/locale/locale.zh.ini
--rwxr-xr-x   0        0        0     1477 2024-03-12 06:49:17.164785 pygpt_net-2.2.1/src/pygpt_net/data/locale/plugin.agent.en.ini
--rwxr-xr-x   0        0        0     1394 2024-03-12 06:49:17.164785 pygpt_net-2.2.1/src/pygpt_net/data/locale/plugin.agent.pl.ini
--rwxr-xr-x   0        0        0     5371 2024-03-12 06:49:17.168786 pygpt_net-2.2.1/src/pygpt_net/data/locale/plugin.audio_input.en.ini
--rwxr-xr-x   0        0        0     5129 2024-03-12 06:49:17.168786 pygpt_net-2.2.1/src/pygpt_net/data/locale/plugin.audio_input.pl.ini
--rwxr-xr-x   0        0        0     1721 2024-03-12 06:49:17.168786 pygpt_net-2.2.1/src/pygpt_net/data/locale/plugin.audio_output.en.ini
--rwxr-xr-x   0        0        0     1395 2024-03-12 06:49:17.168786 pygpt_net-2.2.1/src/pygpt_net/data/locale/plugin.audio_output.pl.ini
--rw-r--r--   0        0        0      622 2024-03-12 06:49:17.168786 pygpt_net-2.2.1/src/pygpt_net/data/locale/plugin.cmd_api.en.ini
--rw-r--r--   0        0        0      853 2024-03-12 06:49:17.168786 pygpt_net-2.2.1/src/pygpt_net/data/locale/plugin.cmd_api.pl.ini
--rwxr-xr-x   0        0        0     2365 2024-03-19 03:42:00.618910 pygpt_net-2.2.1/src/pygpt_net/data/locale/plugin.cmd_code_interpreter.en.ini
--rwxr-xr-x   0        0        0     1614 2024-03-12 06:49:17.168786 pygpt_net-2.2.1/src/pygpt_net/data/locale/plugin.cmd_code_interpreter.pl.ini
--rwxr-xr-x   0        0        0      455 2024-03-12 06:49:17.168786 pygpt_net-2.2.1/src/pygpt_net/data/locale/plugin.cmd_custom.en.ini
--rwxr-xr-x   0        0        0      528 2024-03-12 06:49:17.168786 pygpt_net-2.2.1/src/pygpt_net/data/locale/plugin.cmd_custom.pl.ini
--rwxr-xr-x   0        0        0     4234 2024-03-13 17:35:47.179523 pygpt_net-2.2.1/src/pygpt_net/data/locale/plugin.cmd_files.en.ini
--rwxr-xr-x   0        0        0     3584 2024-03-13 17:35:47.179523 pygpt_net-2.2.1/src/pygpt_net/data/locale/plugin.cmd_files.pl.ini
--rw-r--r--   0        0        0     2280 2024-03-12 06:49:17.168786 pygpt_net-2.2.1/src/pygpt_net/data/locale/plugin.cmd_history.en.ini
--rw-r--r--   0        0        0     2765 2024-03-12 06:49:17.168786 pygpt_net-2.2.1/src/pygpt_net/data/locale/plugin.cmd_history.pl.ini
--rw-r--r--   0        0        0     1042 2024-03-12 06:49:17.168786 pygpt_net-2.2.1/src/pygpt_net/data/locale/plugin.cmd_serial.en.ini
--rw-r--r--   0        0        0     1511 2024-03-12 06:49:17.168786 pygpt_net-2.2.1/src/pygpt_net/data/locale/plugin.cmd_serial.pl.ini
--rwxr-xr-x   0        0        0     4840 2024-03-12 06:49:17.168786 pygpt_net-2.2.1/src/pygpt_net/data/locale/plugin.cmd_web.en.ini
--rwxr-xr-x   0        0        0     4660 2024-03-12 06:49:17.168786 pygpt_net-2.2.1/src/pygpt_net/data/locale/plugin.cmd_web.pl.ini
--rw-r--r--   0        0        0      758 2024-03-12 06:49:17.168786 pygpt_net-2.2.1/src/pygpt_net/data/locale/plugin.crontab.en.ini
--rw-r--r--   0        0        0      871 2024-03-12 06:49:17.168786 pygpt_net-2.2.1/src/pygpt_net/data/locale/plugin.crontab.pl.ini
--rw-r--r--   0        0        0      338 2024-03-12 06:49:17.168786 pygpt_net-2.2.1/src/pygpt_net/data/locale/plugin.extra_prompt.en.ini
--rw-r--r--   0        0        0      474 2024-03-12 03:34:38.663323 pygpt_net-2.2.1/src/pygpt_net/data/locale/plugin.extra_prompt.pl.ini
--rwxr-xr-x   0        0        0     1970 2024-03-13 17:35:47.179523 pygpt_net-2.2.1/src/pygpt_net/data/locale/plugin.idx_llama_index.en.ini
--rwxr-xr-x   0        0        0     1180 2024-03-13 17:35:47.179523 pygpt_net-2.2.1/src/pygpt_net/data/locale/plugin.idx_llama_index.pl.ini
--rw-r--r--   0        0        0      396 2024-03-17 13:18:45.662349 pygpt_net-2.2.1/src/pygpt_net/data/locale/plugin.openai_dalle.en.ini
--rw-r--r--   0        0        0      427 2024-03-17 13:18:45.662349 pygpt_net-2.2.1/src/pygpt_net/data/locale/plugin.openai_dalle.pl.ini
--rw-r--r--   0        0        0     1393 2024-03-12 06:49:17.168786 pygpt_net-2.2.1/src/pygpt_net/data/locale/plugin.openai_vision.en.ini
--rw-r--r--   0        0        0     1426 2024-03-12 06:49:17.168786 pygpt_net-2.2.1/src/pygpt_net/data/locale/plugin.openai_vision.pl.ini
--rwxr-xr-x   0        0        0      631 2024-01-30 20:56:32.776879 pygpt_net-2.2.1/src/pygpt_net/data/locale/plugin.real_time.en.ini
--rwxr-xr-x   0        0        0      752 2024-01-30 20:56:32.776879 pygpt_net-2.2.1/src/pygpt_net/data/locale/plugin.real_time.pl.ini
--rwxr-xr-x   0        0        0    19418 2023-12-14 19:08:45.000000 pygpt_net-2.2.1/src/pygpt_net/data/logo.png
--rw-r--r--   0        0        0    83051 2024-04-22 22:35:26.800429 pygpt_net-2.2.1/src/pygpt_net/data/prompts.csv
--rwxr-xr-x   0        0        0    31708 2024-02-20 19:10:03.189314 pygpt_net-2.2.1/src/pygpt_net/data/win32/README.rtf
--rwxr-xr-x   0        0        0     1633 2023-04-14 00:10:28.000000 pygpt_net-2.2.1/src/pygpt_net/data/win32/USER-LICENSE.rtf
--rwxr-xr-x   0        0        0    87160 2023-04-14 00:10:28.000000 pygpt_net-2.2.1/src/pygpt_net/data/win32/pygpt.aip
--rwxr-xr-x   0        0        0       45 2023-12-19 15:40:13.000000 pygpt_net-2.2.1/src/pygpt_net/data/win32/qt.conf
--rw-r--r--   0        0        0    21736 2024-03-02 20:04:01.386329 pygpt_net-2.2.1/src/pygpt_net/icons.qrc
--rw-r--r--   0        0        0    90430 2024-03-02 20:05:43.048414 pygpt_net-2.2.1/src/pygpt_net/icons_rc.py
--rw-r--r--   0        0        0      488 2023-12-31 03:12:36.955235 pygpt_net-2.2.1/src/pygpt_net/item/__init__.py
--rw-r--r--   0        0        0     9587 2024-04-26 21:55:50.679597 pygpt_net-2.2.1/src/pygpt_net/item/assistant.py
--rw-r--r--   0        0        0     2110 2024-04-26 21:55:50.679597 pygpt_net-2.2.1/src/pygpt_net/item/attachment.py
--rw-r--r--   0        0        0     2108 2024-01-27 21:42:30.960980 pygpt_net-2.2.1/src/pygpt_net/item/calendar_note.py
--rw-r--r--   0        0        0    11455 2024-04-10 01:07:30.188635 pygpt_net-2.2.1/src/pygpt_net/item/ctx.py
--rw-r--r--   0        0        0     1681 2024-01-27 21:42:30.960980 pygpt_net-2.2.1/src/pygpt_net/item/index.py
--rw-r--r--   0        0        0      600 2023-12-31 03:12:34.283242 pygpt_net-2.2.1/src/pygpt_net/item/mode.py
--rw-r--r--   0        0        0     6208 2024-01-27 21:42:30.960980 pygpt_net-2.2.1/src/pygpt_net/item/model.py
--rw-r--r--   0        0        0     1508 2024-01-27 21:42:30.960980 pygpt_net-2.2.1/src/pygpt_net/item/notepad.py
--rw-r--r--   0        0        0     4052 2024-02-15 05:07:04.122540 pygpt_net-2.2.1/src/pygpt_net/item/preset.py
--rwxr-xr-x   0        0        0     7995 2024-04-21 18:06:27.128064 pygpt_net-2.2.1/src/pygpt_net/launcher.py
--rw-r--r--   0        0        0     2849 2023-12-28 02:55:13.572642 pygpt_net-2.2.1/src/pygpt_net/migrations/Version20231227152900.py
--rw-r--r--   0        0        0      906 2023-12-30 08:47:37.360628 pygpt_net-2.2.1/src/pygpt_net/migrations/Version20231230095000.py
--rw-r--r--   0        0        0      901 2024-01-01 00:17:57.553256 pygpt_net-2.2.1/src/pygpt_net/migrations/Version20231231230000.py
--rw-r--r--   0        0        0     1303 2024-01-06 06:27:36.351928 pygpt_net-2.2.1/src/pygpt_net/migrations/Version20240106060000.py
--rw-r--r--   0        0        0      865 2024-01-07 09:35:02.638810 pygpt_net-2.2.1/src/pygpt_net/migrations/Version20240107060000.py
--rw-r--r--   0        0        0     1756 2024-02-23 01:50:39.602419 pygpt_net-2.2.1/src/pygpt_net/migrations/Version20240222160000.py
--rw-r--r--   0        0        0     1099 2024-02-23 06:06:25.510176 pygpt_net-2.2.1/src/pygpt_net/migrations/Version20240223050000.py
--rw-r--r--   0        0        0      847 2024-03-03 22:43:17.403437 pygpt_net-2.2.1/src/pygpt_net/migrations/Version20240303190000.py
--rw-r--r--   0        0        0     1110 2024-04-10 01:07:30.188635 pygpt_net-2.2.1/src/pygpt_net/migrations/Version20240408180000.py
--rw-r--r--   0        0        0     1745 2024-04-26 21:55:50.679597 pygpt_net-2.2.1/src/pygpt_net/migrations/Version20240426050000.py
--rw-r--r--   0        0        0     1862 2024-04-26 21:55:50.679597 pygpt_net-2.2.1/src/pygpt_net/migrations/__init__.py
--rw-r--r--   0        0        0      614 2023-12-28 02:55:13.572642 pygpt_net-2.2.1/src/pygpt_net/migrations/base.py
--rwxr-xr-x   0        0        0      488 2023-12-25 22:13:46.802302 pygpt_net-2.2.1/src/pygpt_net/plugin/__init__.py
--rwxr-xr-x   0        0        0    15161 2024-03-07 01:04:26.445956 pygpt_net-2.2.1/src/pygpt_net/plugin/agent/__init__.py
--rwxr-xr-x   0        0        0    23567 2024-03-26 17:12:51.294309 pygpt_net-2.2.1/src/pygpt_net/plugin/audio_input/__init__.py
--rw-r--r--   0        0        0     4669 2024-04-24 23:37:32.612565 pygpt_net-2.2.1/src/pygpt_net/plugin/audio_input/simple.py
--rwxr-xr-x   0        0        0    10466 2024-03-19 09:04:41.054930 pygpt_net-2.2.1/src/pygpt_net/plugin/audio_input/worker.py
--rwxr-xr-x   0        0        0     6940 2024-03-10 10:31:05.897000 pygpt_net-2.2.1/src/pygpt_net/plugin/audio_output/__init__.py
--rw-r--r--   0        0        0     1806 2024-03-10 10:31:05.897000 pygpt_net-2.2.1/src/pygpt_net/plugin/audio_output/worker.py
--rwxr-xr-x   0        0        0    12704 2024-03-18 04:54:07.637826 pygpt_net-2.2.1/src/pygpt_net/plugin/base.py
--rwxr-xr-x   0        0        0    11734 2024-03-12 06:49:17.168786 pygpt_net-2.2.1/src/pygpt_net/plugin/cmd_api/__init__.py
--rw-r--r--   0        0        0     6243 2024-03-16 12:28:31.211383 pygpt_net-2.2.1/src/pygpt_net/plugin/cmd_api/worker.py
--rwxr-xr-x   0        0        0     9571 2024-03-26 17:12:51.294309 pygpt_net-2.2.1/src/pygpt_net/plugin/cmd_code_interpreter/__init__.py
--rw-r--r--   0        0        0    14580 2024-04-28 01:03:40.864507 pygpt_net-2.2.1/src/pygpt_net/plugin/cmd_code_interpreter/runner.py
--rw-r--r--   0        0        0     8841 2024-04-28 01:03:50.072481 pygpt_net-2.2.1/src/pygpt_net/plugin/cmd_code_interpreter/worker.py
--rwxr-xr-x   0        0        0     5875 2024-03-12 06:49:17.168786 pygpt_net-2.2.1/src/pygpt_net/plugin/cmd_custom/__init__.py
--rw-r--r--   0        0        0     4507 2024-03-16 12:28:31.211383 pygpt_net-2.2.1/src/pygpt_net/plugin/cmd_custom/worker.py
--rwxr-xr-x   0        0        0    17031 2024-04-25 01:16:54.112014 pygpt_net-2.2.1/src/pygpt_net/plugin/cmd_files/__init__.py
--rwxr-xr-x   0        0        0    37969 2024-04-25 01:16:54.112014 pygpt_net-2.2.1/src/pygpt_net/plugin/cmd_files/worker.py
--rwxr-xr-x   0        0        0    20140 2024-03-16 12:28:31.211383 pygpt_net-2.2.1/src/pygpt_net/plugin/cmd_history/__init__.py
--rw-r--r--   0        0        0     6673 2024-03-16 12:28:31.211383 pygpt_net-2.2.1/src/pygpt_net/plugin/cmd_history/worker.py
--rwxr-xr-x   0        0        0     6124 2024-03-16 12:28:31.211383 pygpt_net-2.2.1/src/pygpt_net/plugin/cmd_serial/__init__.py
--rw-r--r--   0        0        0     8562 2024-03-16 12:28:31.211383 pygpt_net-2.2.1/src/pygpt_net/plugin/cmd_serial/worker.py
--rwxr-xr-x   0        0        0    21060 2024-03-17 14:26:02.923314 pygpt_net-2.2.1/src/pygpt_net/plugin/cmd_web/__init__.py
--rwxr-xr-x   0        0        0    12576 2024-02-24 01:55:58.445111 pygpt_net-2.2.1/src/pygpt_net/plugin/cmd_web/websearch.py
--rw-r--r--   0        0        0    10794 2024-03-26 17:12:51.294309 pygpt_net-2.2.1/src/pygpt_net/plugin/cmd_web/worker.py
--rwxr-xr-x   0        0        0     8163 2024-03-15 15:31:21.786121 pygpt_net-2.2.1/src/pygpt_net/plugin/crontab/__init__.py
--rwxr-xr-x   0        0        0     2831 2024-02-18 01:14:49.758062 pygpt_net-2.2.1/src/pygpt_net/plugin/extra_prompt/__init__.py
--rwxr-xr-x   0        0        0    14334 2024-04-17 01:35:30.426055 pygpt_net-2.2.1/src/pygpt_net/plugin/idx_llama_index/__init__.py
--rw-r--r--   0        0        0     2825 2024-03-16 16:19:22.432875 pygpt_net-2.2.1/src/pygpt_net/plugin/idx_llama_index/worker.py
--rwxr-xr-x   0        0        0     6272 2024-03-17 13:18:45.662349 pygpt_net-2.2.1/src/pygpt_net/plugin/openai_dalle/__init__.py
--rwxr-xr-x   0        0        0    11659 2024-04-11 20:50:24.193030 pygpt_net-2.2.1/src/pygpt_net/plugin/openai_vision/__init__.py
--rwxr-xr-x   0        0        0     3865 2024-03-17 13:18:45.662349 pygpt_net-2.2.1/src/pygpt_net/plugin/real_time/__init__.py
--rw-r--r--   0        0        0      488 2023-12-25 22:13:46.802302 pygpt_net-2.2.1/src/pygpt_net/provider/__init__.py
--rw-r--r--   0        0        0      488 2024-02-24 01:55:58.445111 pygpt_net-2.2.1/src/pygpt_net/provider/audio_input/__init__.py
--rw-r--r--   0        0        0     1819 2024-02-27 05:21:39.771084 pygpt_net-2.2.1/src/pygpt_net/provider/audio_input/base.py
--rw-r--r--   0        0        0     2818 2024-02-27 05:21:39.771084 pygpt_net-2.2.1/src/pygpt_net/provider/audio_input/bing_speech_recognition.py
--rw-r--r--   0        0        0     2904 2024-02-27 05:21:39.771084 pygpt_net-2.2.1/src/pygpt_net/provider/audio_input/google_cloud_speech_recognition.py
--rw-r--r--   0        0        0     2840 2024-02-27 05:21:39.771084 pygpt_net-2.2.1/src/pygpt_net/provider/audio_input/google_speech_recognition.py
--rw-r--r--   0        0        0     2244 2024-03-01 03:17:53.457929 pygpt_net-2.2.1/src/pygpt_net/provider/audio_input/openai_whisper.py
--rw-r--r--   0        0        0     3129 2024-03-01 03:17:53.457929 pygpt_net-2.2.1/src/pygpt_net/provider/audio_input/openai_whisper_local.py
--rw-r--r--   0        0        0      488 2024-02-24 01:55:58.449111 pygpt_net-2.2.1/src/pygpt_net/provider/audio_output/__init__.py
--rw-r--r--   0        0        0     1995 2024-02-27 05:21:39.771084 pygpt_net-2.2.1/src/pygpt_net/provider/audio_output/base.py
--rw-r--r--   0        0        0     4231 2024-02-25 00:27:02.862945 pygpt_net-2.2.1/src/pygpt_net/provider/audio_output/eleven_labs.py
--rw-r--r--   0        0        0     4286 2024-02-25 00:27:02.862945 pygpt_net-2.2.1/src/pygpt_net/provider/audio_output/google_tts.py
--rw-r--r--   0        0        0     4960 2024-02-24 01:55:58.449111 pygpt_net-2.2.1/src/pygpt_net/provider/audio_output/ms_azure_tts.py
--rw-r--r--   0        0        0     3056 2024-02-24 01:55:58.449111 pygpt_net-2.2.1/src/pygpt_net/provider/audio_output/openai_tts.py
--rw-r--r--   0        0        0      488 2024-01-23 23:46:30.499197 pygpt_net-2.2.1/src/pygpt_net/provider/core/__init__.py
--rw-r--r--   0        0        0      488 2024-01-23 23:46:30.499197 pygpt_net-2.2.1/src/pygpt_net/provider/core/assistant/__init__.py
--rw-r--r--   0        0        0     1186 2024-01-23 23:46:30.499197 pygpt_net-2.2.1/src/pygpt_net/provider/core/assistant/base.py
--rw-r--r--   0        0        0     6399 2024-04-26 21:55:50.679597 pygpt_net-2.2.1/src/pygpt_net/provider/core/assistant/json_file.py
--rw-r--r--   0        0        0      488 2024-04-26 21:55:50.679597 pygpt_net-2.2.1/src/pygpt_net/provider/core/assistant_file/__init__.py
--rw-r--r--   0        0        0     1291 2024-04-26 21:55:50.679597 pygpt_net-2.2.1/src/pygpt_net/provider/core/assistant_file/base.py
--rw-r--r--   0        0        0     5125 2024-04-26 21:55:50.679597 pygpt_net-2.2.1/src/pygpt_net/provider/core/assistant_file/db_sqlite/__init__.py
--rw-r--r--   0        0        0      885 2024-04-26 21:55:50.679597 pygpt_net-2.2.1/src/pygpt_net/provider/core/assistant_file/db_sqlite/patch.py
--rw-r--r--   0        0        0    10392 2024-04-26 21:55:50.679597 pygpt_net-2.2.1/src/pygpt_net/provider/core/assistant_file/db_sqlite/storage.py
--rw-r--r--   0        0        0     1796 2024-04-26 21:55:50.679597 pygpt_net-2.2.1/src/pygpt_net/provider/core/assistant_file/db_sqlite/utils.py
--rw-r--r--   0        0        0      488 2024-04-26 21:55:50.679597 pygpt_net-2.2.1/src/pygpt_net/provider/core/assistant_store/__init__.py
--rw-r--r--   0        0        0     1314 2024-04-26 21:55:50.679597 pygpt_net-2.2.1/src/pygpt_net/provider/core/assistant_store/base.py
--rw-r--r--   0        0        0     3557 2024-04-26 21:55:50.679597 pygpt_net-2.2.1/src/pygpt_net/provider/core/assistant_store/db_sqlite/__init__.py
--rw-r--r--   0        0        0      885 2024-04-26 21:55:50.679597 pygpt_net-2.2.1/src/pygpt_net/provider/core/assistant_store/db_sqlite/patch.py
--rw-r--r--   0        0        0     7438 2024-04-26 21:55:50.679597 pygpt_net-2.2.1/src/pygpt_net/provider/core/assistant_store/db_sqlite/storage.py
--rw-r--r--   0        0        0     2120 2024-04-26 21:55:50.679597 pygpt_net-2.2.1/src/pygpt_net/provider/core/assistant_store/db_sqlite/utils.py
--rw-r--r--   0        0        0     4377 2024-04-26 21:55:50.679597 pygpt_net-2.2.1/src/pygpt_net/provider/core/assistant_store/json_file.py
--rw-r--r--   0        0        0      488 2024-01-23 23:46:30.499197 pygpt_net-2.2.1/src/pygpt_net/provider/core/attachment/__init__.py
--rw-r--r--   0        0        0     1204 2024-01-23 23:46:30.499197 pygpt_net-2.2.1/src/pygpt_net/provider/core/attachment/base.py
--rw-r--r--   0        0        0     5404 2024-04-26 21:55:50.679597 pygpt_net-2.2.1/src/pygpt_net/provider/core/attachment/json_file.py
--rw-r--r--   0        0        0      488 2024-01-23 23:46:30.499197 pygpt_net-2.2.1/src/pygpt_net/provider/core/calendar/__init__.py
--rw-r--r--   0        0        0     1322 2024-01-23 23:46:30.499197 pygpt_net-2.2.1/src/pygpt_net/provider/core/calendar/base.py
--rw-r--r--   0        0        0     3953 2024-03-08 00:36:17.343108 pygpt_net-2.2.1/src/pygpt_net/provider/core/calendar/db_sqlite/__init__.py
--rw-r--r--   0        0        0      837 2024-01-23 23:46:30.499197 pygpt_net-2.2.1/src/pygpt_net/provider/core/calendar/db_sqlite/patch.py
--rw-r--r--   0        0        0    11113 2024-03-07 01:04:26.445956 pygpt_net-2.2.1/src/pygpt_net/provider/core/calendar/db_sqlite/storage.py
--rw-r--r--   0        0        0      488 2024-01-23 23:46:30.499197 pygpt_net-2.2.1/src/pygpt_net/provider/core/config/__init__.py
--rw-r--r--   0        0        0     1235 2024-01-23 23:46:30.499197 pygpt_net-2.2.1/src/pygpt_net/provider/core/config/base.py
--rwxr-xr-x   0        0        0     5017 2024-04-11 01:27:21.134184 pygpt_net-2.2.1/src/pygpt_net/provider/core/config/json_file.py
--rwxr-xr-x   0        0        0    75483 2024-04-26 21:55:50.679597 pygpt_net-2.2.1/src/pygpt_net/provider/core/config/patch.py
--rw-r--r--   0        0        0      488 2024-01-23 23:46:30.499197 pygpt_net-2.2.1/src/pygpt_net/provider/core/ctx/__init__.py
--rw-r--r--   0        0        0     2577 2024-04-17 05:13:33.075416 pygpt_net-2.2.1/src/pygpt_net/provider/core/ctx/base.py
--rw-r--r--   0        0        0     9171 2024-04-17 05:13:33.075416 pygpt_net-2.2.1/src/pygpt_net/provider/core/ctx/db_sqlite/__init__.py
--rw-r--r--   0        0        0     3101 2024-01-23 23:46:30.499197 pygpt_net-2.2.1/src/pygpt_net/provider/core/ctx/db_sqlite/patch.py
--rw-r--r--   0        0        0    31650 2024-04-17 05:13:33.075416 pygpt_net-2.2.1/src/pygpt_net/provider/core/ctx/db_sqlite/storage.py
--rw-r--r--   0        0        0     7644 2024-04-10 01:07:30.188635 pygpt_net-2.2.1/src/pygpt_net/provider/core/ctx/db_sqlite/utils.py
--rw-r--r--   0        0        0    11665 2024-01-23 23:46:30.503197 pygpt_net-2.2.1/src/pygpt_net/provider/core/ctx/json_file.py
--rw-r--r--   0        0        0      488 2024-01-23 23:46:30.503197 pygpt_net-2.2.1/src/pygpt_net/provider/core/history/__init__.py
--rw-r--r--   0        0        0      863 2024-01-23 23:46:30.503197 pygpt_net-2.2.1/src/pygpt_net/provider/core/history/base.py
--rw-r--r--   0        0        0      837 2024-01-23 23:46:30.503197 pygpt_net-2.2.1/src/pygpt_net/provider/core/history/patch.py
--rw-r--r--   0        0        0     2969 2024-01-23 23:46:30.503197 pygpt_net-2.2.1/src/pygpt_net/provider/core/history/txt_file.py
--rw-r--r--   0        0        0      488 2024-01-23 23:46:30.503197 pygpt_net-2.2.1/src/pygpt_net/provider/core/index/__init__.py
--rw-r--r--   0        0        0     2875 2024-03-07 01:04:26.445956 pygpt_net-2.2.1/src/pygpt_net/provider/core/index/base.py
--rw-r--r--   0        0        0     8502 2024-03-07 01:04:26.445956 pygpt_net-2.2.1/src/pygpt_net/provider/core/index/db_sqlite/__init__.py
--rw-r--r--   0        0        0     2972 2024-02-23 06:06:25.510176 pygpt_net-2.2.1/src/pygpt_net/provider/core/index/db_sqlite/patch.py
--rw-r--r--   0        0        0    17470 2024-03-07 01:04:26.445956 pygpt_net-2.2.1/src/pygpt_net/provider/core/index/db_sqlite/storage.py
--rw-r--r--   0        0        0      934 2024-03-07 01:04:26.445956 pygpt_net-2.2.1/src/pygpt_net/provider/core/index/db_sqlite/utils.py
--rw-r--r--   0        0        0     6615 2024-02-23 01:50:39.606418 pygpt_net-2.2.1/src/pygpt_net/provider/core/index/json_file.py
--rw-r--r--   0        0        0      837 2024-01-23 23:46:30.503197 pygpt_net-2.2.1/src/pygpt_net/provider/core/index/patch.py
--rw-r--r--   0        0        0      488 2024-01-23 23:46:30.503197 pygpt_net-2.2.1/src/pygpt_net/provider/core/mode/__init__.py
--rw-r--r--   0        0        0     1062 2024-01-23 23:46:30.503197 pygpt_net-2.2.1/src/pygpt_net/provider/core/mode/base.py
--rw-r--r--   0        0        0     4142 2024-01-23 23:46:30.503197 pygpt_net-2.2.1/src/pygpt_net/provider/core/mode/json_file.py
--rw-r--r--   0        0        0      837 2024-01-23 23:46:30.503197 pygpt_net-2.2.1/src/pygpt_net/provider/core/mode/patch.py
--rw-r--r--   0        0        0      488 2024-01-23 23:46:30.503197 pygpt_net-2.2.1/src/pygpt_net/provider/core/model/__init__.py
--rw-r--r--   0        0        0     1246 2024-01-23 23:46:30.503197 pygpt_net-2.2.1/src/pygpt_net/provider/core/model/base.py
--rw-r--r--   0        0        0     6231 2024-01-23 23:46:30.503197 pygpt_net-2.2.1/src/pygpt_net/provider/core/model/json_file.py
--rw-r--r--   0        0        0     9769 2024-04-11 20:50:24.193030 pygpt_net-2.2.1/src/pygpt_net/provider/core/model/patch.py
--rw-r--r--   0        0        0      488 2024-01-23 23:46:30.503197 pygpt_net-2.2.1/src/pygpt_net/provider/core/notepad/__init__.py
--rw-r--r--   0        0        0     1262 2024-01-23 23:46:30.503197 pygpt_net-2.2.1/src/pygpt_net/provider/core/notepad/base.py
--rw-r--r--   0        0        0     3044 2024-01-23 23:46:30.503197 pygpt_net-2.2.1/src/pygpt_net/provider/core/notepad/db_sqlite/__init__.py
--rw-r--r--   0        0        0     2805 2024-01-23 23:46:30.503197 pygpt_net-2.2.1/src/pygpt_net/provider/core/notepad/db_sqlite/patch.py
--rw-r--r--   0        0        0     7263 2024-01-23 23:46:30.503197 pygpt_net-2.2.1/src/pygpt_net/provider/core/notepad/db_sqlite/storage.py
--rw-r--r--   0        0        0     7555 2024-01-23 23:46:30.503197 pygpt_net-2.2.1/src/pygpt_net/provider/core/notepad/json_file.py
--rw-r--r--   0        0        0      488 2024-03-07 01:04:26.445956 pygpt_net-2.2.1/src/pygpt_net/provider/core/plugin_preset/__init__.py
--rw-r--r--   0        0        0      987 2024-03-07 01:04:26.445956 pygpt_net-2.2.1/src/pygpt_net/provider/core/plugin_preset/base.py
--rwxr-xr-x   0        0        0     3198 2024-03-07 01:04:26.445956 pygpt_net-2.2.1/src/pygpt_net/provider/core/plugin_preset/json_file.py
--rwxr-xr-x   0        0        0     1766 2024-03-07 01:04:26.445956 pygpt_net-2.2.1/src/pygpt_net/provider/core/plugin_preset/patch.py
--rwxr-xr-x   0        0        0      488 2024-01-23 23:46:30.503197 pygpt_net-2.2.1/src/pygpt_net/provider/core/preset/__init__.py
--rwxr-xr-x   0        0        0     1300 2024-02-01 01:48:09.374583 pygpt_net-2.2.1/src/pygpt_net/provider/core/preset/base.py
--rwxr-xr-x   0        0        0     7887 2024-02-15 05:07:04.122540 pygpt_net-2.2.1/src/pygpt_net/provider/core/preset/json_file.py
--rw-r--r--   0        0        0     3166 2024-01-23 23:46:30.503197 pygpt_net-2.2.1/src/pygpt_net/provider/core/preset/patch.py
--rw-r--r--   0        0        0     6961 2024-03-08 00:36:17.343108 pygpt_net-2.2.1/src/pygpt_net/provider/gpt/__init__.py
--rw-r--r--   0        0        0    26543 2024-04-26 21:55:50.679597 pygpt_net-2.2.1/src/pygpt_net/provider/gpt/assistants.py
--rw-r--r--   0        0        0     5763 2024-03-08 00:03:22.338417 pygpt_net-2.2.1/src/pygpt_net/provider/gpt/chat.py
--rw-r--r--   0        0        0     5354 2024-03-09 21:41:28.193853 pygpt_net-2.2.1/src/pygpt_net/provider/gpt/completion.py
--rw-r--r--   0        0        0     7903 2024-03-17 13:18:45.662349 pygpt_net-2.2.1/src/pygpt_net/provider/gpt/image.py
--rw-r--r--   0        0        0     1848 2024-03-17 13:18:45.662349 pygpt_net-2.2.1/src/pygpt_net/provider/gpt/summarizer.py
--rw-r--r--   0        0        0     7341 2024-03-12 21:25:35.838043 pygpt_net-2.2.1/src/pygpt_net/provider/gpt/vision.py
--rw-r--r--   0        0        0        0 2024-02-20 19:10:03.189314 pygpt_net-2.2.1/src/pygpt_net/provider/gpt/worker/__init__.py
--rw-r--r--   0        0        0    15828 2024-04-28 06:16:26.324027 pygpt_net-2.2.1/src/pygpt_net/provider/gpt/worker/assistants.py
--rw-r--r--   0        0        0    10157 2024-04-27 07:58:32.750704 pygpt_net-2.2.1/src/pygpt_net/provider/gpt/worker/importer.py
--rwxr-xr-x   0        0        0        0 2024-01-27 21:42:30.960980 pygpt_net-2.2.1/src/pygpt_net/provider/llms/__init__.py
--rwxr-xr-x   0        0        0     1641 2024-01-27 21:42:30.960980 pygpt_net-2.2.1/src/pygpt_net/provider/llms/anthropic.py
--rwxr-xr-x   0        0        0     2800 2024-03-13 15:08:01.569797 pygpt_net-2.2.1/src/pygpt_net/provider/llms/azure_openai.py
--rw-r--r--   0        0        0     3940 2024-03-15 15:31:21.790122 pygpt_net-2.2.1/src/pygpt_net/provider/llms/base.py
--rwxr-xr-x   0        0        0     1535 2024-01-27 21:42:30.960980 pygpt_net-2.2.1/src/pygpt_net/provider/llms/hugging_face.py
--rwxr-xr-x   0        0        0     1643 2024-01-27 21:42:30.960980 pygpt_net-2.2.1/src/pygpt_net/provider/llms/llama.py
--rwxr-xr-x   0        0        0     1517 2024-01-27 21:42:30.960980 pygpt_net-2.2.1/src/pygpt_net/provider/llms/ollama.py
--rwxr-xr-x   0        0        0     2727 2024-03-13 15:08:01.569797 pygpt_net-2.2.1/src/pygpt_net/provider/llms/openai.py
--rw-r--r--   0        0        0        0 2024-01-23 23:46:30.503197 pygpt_net-2.2.1/src/pygpt_net/provider/loaders/__init__.py
--rw-r--r--   0        0        0     2515 2024-04-17 01:35:30.426055 pygpt_net-2.2.1/src/pygpt_net/provider/loaders/base.py
--rw-r--r--   0        0        0     1258 2024-04-17 01:35:30.426055 pygpt_net-2.2.1/src/pygpt_net/provider/loaders/file_csv.py
--rw-r--r--   0        0        0     1032 2024-02-29 03:07:51.278132 pygpt_net-2.2.1/src/pygpt_net/provider/loaders/file_docx.py
--rw-r--r--   0        0        0     1022 2024-02-29 03:07:51.278132 pygpt_net-2.2.1/src/pygpt_net/provider/loaders/file_epub.py
--rw-r--r--   0        0        0     1032 2024-02-28 03:58:59.309445 pygpt_net-2.2.1/src/pygpt_net/provider/loaders/file_excel.py
--rw-r--r--   0        0        0     1268 2024-04-17 01:35:30.426055 pygpt_net-2.2.1/src/pygpt_net/provider/loaders/file_html.py
--rw-r--r--   0        0        0     1923 2024-04-17 01:35:30.426055 pygpt_net-2.2.1/src/pygpt_net/provider/loaders/file_image_vision.py
--rw-r--r--   0        0        0     1284 2024-04-17 01:35:30.426055 pygpt_net-2.2.1/src/pygpt_net/provider/loaders/file_ipynb.py
--rw-r--r--   0        0        0      996 2024-02-28 03:58:59.309445 pygpt_net-2.2.1/src/pygpt_net/provider/loaders/file_json.py
--rw-r--r--   0        0        0     1292 2024-04-17 01:35:30.426055 pygpt_net-2.2.1/src/pygpt_net/provider/loaders/file_markdown.py
--rw-r--r--   0        0        0     1214 2024-04-17 01:35:30.426055 pygpt_net-2.2.1/src/pygpt_net/provider/loaders/file_pdf.py
--rw-r--r--   0        0        0     1832 2024-04-17 01:35:30.426055 pygpt_net-2.2.1/src/pygpt_net/provider/loaders/file_video_audio.py
--rw-r--r--   0        0        0     1196 2024-04-17 01:35:30.426055 pygpt_net-2.2.1/src/pygpt_net/provider/loaders/file_xml.py
--rw-r--r--   0        0        0        0 2024-01-27 21:42:30.960980 pygpt_net-2.2.1/src/pygpt_net/provider/loaders/hub/__init__.py
--rw-r--r--   0        0        0        0 2024-03-01 17:40:19.825274 pygpt_net-2.2.1/src/pygpt_net/provider/loaders/hub/bitbucket/__init__.py
--rw-r--r--   0        0        0     6194 2024-03-01 17:40:19.825274 pygpt_net-2.2.1/src/pygpt_net/provider/loaders/hub/bitbucket/repo.py
--rw-r--r--   0        0        0        0 2024-03-01 17:40:19.825274 pygpt_net-2.2.1/src/pygpt_net/provider/loaders/hub/chatgpt_retrieval/__init__.py
--rw-r--r--   0        0        0     2460 2024-03-01 17:40:19.825274 pygpt_net-2.2.1/src/pygpt_net/provider/loaders/hub/chatgpt_retrieval/base.py
--rw-r--r--   0        0        0        0 2024-03-01 17:40:19.825274 pygpt_net-2.2.1/src/pygpt_net/provider/loaders/hub/database/__init__.py
--rw-r--r--   0        0        0     4228 2024-03-01 17:40:19.825274 pygpt_net-2.2.1/src/pygpt_net/provider/loaders/hub/database/base.py
--rw-r--r--   0        0        0        0 2024-03-01 17:40:19.825274 pygpt_net-2.2.1/src/pygpt_net/provider/loaders/hub/github/__init__.py
--rw-r--r--   0        0        0     4204 2024-03-01 17:40:19.825274 pygpt_net-2.2.1/src/pygpt_net/provider/loaders/hub/github/issues.py
--rw-r--r--   0        0        0     3550 2024-03-01 17:40:19.825274 pygpt_net-2.2.1/src/pygpt_net/provider/loaders/hub/github/repo.py
--rw-r--r--   0        0        0        0 2024-03-01 03:17:53.457929 pygpt_net-2.2.1/src/pygpt_net/provider/loaders/hub/google/__init__.py
--rw-r--r--   0        0        0     2658 2024-03-01 03:17:53.457929 pygpt_net-2.2.1/src/pygpt_net/provider/loaders/hub/google/calendar.py
--rw-r--r--   0        0        0     5370 2024-03-01 03:17:53.457929 pygpt_net-2.2.1/src/pygpt_net/provider/loaders/hub/google/docs.py
--rw-r--r--   0        0        0     6772 2024-03-01 03:17:53.457929 pygpt_net-2.2.1/src/pygpt_net/provider/loaders/hub/google/gmail.py
--rw-r--r--   0        0        0     1633 2024-03-01 03:17:53.457929 pygpt_net-2.2.1/src/pygpt_net/provider/loaders/hub/google/keep.py
--rw-r--r--   0        0        0     5282 2024-03-01 03:17:53.457929 pygpt_net-2.2.1/src/pygpt_net/provider/loaders/hub/google/sheets.py
--rw-r--r--   0        0        0        0 2024-03-01 03:17:53.457929 pygpt_net-2.2.1/src/pygpt_net/provider/loaders/hub/image_vision/__init__.py
--rw-r--r--   0        0        0     6940 2024-03-01 03:17:53.457929 pygpt_net-2.2.1/src/pygpt_net/provider/loaders/hub/image_vision/base.py
--rw-r--r--   0        0        0        0 2024-01-27 21:42:30.964980 pygpt_net-2.2.1/src/pygpt_net/provider/loaders/hub/json/__init__.py
--rw-r--r--   0        0        0     3862 2024-02-29 03:07:51.278132 pygpt_net-2.2.1/src/pygpt_net/provider/loaders/hub/json/base.py
--rw-r--r--   0        0        0        0 2024-01-27 21:42:30.964980 pygpt_net-2.2.1/src/pygpt_net/provider/loaders/hub/pandas_excel/__init__.py
--rw-r--r--   0        0        0     3940 2024-02-29 03:07:51.278132 pygpt_net-2.2.1/src/pygpt_net/provider/loaders/hub/pandas_excel/base.py
--rw-r--r--   0        0        0        0 2024-01-27 21:42:30.964980 pygpt_net-2.2.1/src/pygpt_net/provider/loaders/hub/simple_csv/__init__.py
--rw-r--r--   0        0        0     1481 2024-02-29 03:07:51.278132 pygpt_net-2.2.1/src/pygpt_net/provider/loaders/hub/simple_csv/base.py
--rw-r--r--   0        0        0        0 2024-03-01 03:17:53.457929 pygpt_net-2.2.1/src/pygpt_net/provider/loaders/hub/video_audio/__init__.py
--rw-r--r--   0        0        0     4960 2024-03-01 03:17:53.457929 pygpt_net-2.2.1/src/pygpt_net/provider/loaders/hub/video_audio/base.py
--rw-r--r--   0        0        0        0 2024-02-27 05:21:39.771084 pygpt_net-2.2.1/src/pygpt_net/provider/loaders/hub/web_page/__init__.py
--rw-r--r--   0        0        0      556 2024-02-29 03:07:51.278132 pygpt_net-2.2.1/src/pygpt_net/provider/loaders/hub/web_page/base.py
--rw-r--r--   0        0        0        0 2024-02-27 05:21:39.771084 pygpt_net-2.2.1/src/pygpt_net/provider/loaders/hub/yt/__init__.py
--rw-r--r--   0        0        0     2427 2024-02-29 03:07:51.278132 pygpt_net-2.2.1/src/pygpt_net/provider/loaders/hub/yt/base.py
--rw-r--r--   0        0        0      545 2024-02-27 05:21:39.771084 pygpt_net-2.2.1/src/pygpt_net/provider/loaders/hub/yt/utils.py
--rw-r--r--   0        0        0     3626 2024-04-17 01:35:30.426055 pygpt_net-2.2.1/src/pygpt_net/provider/loaders/web_bitbucket.py
--rw-r--r--   0        0        0     2580 2024-04-17 01:35:30.426055 pygpt_net-2.2.1/src/pygpt_net/provider/loaders/web_chatgpt_retrieval.py
--rw-r--r--   0        0        0     2834 2024-04-17 01:35:30.426055 pygpt_net-2.2.1/src/pygpt_net/provider/loaders/web_database.py
--rw-r--r--   0        0        0     3832 2024-04-17 01:35:30.426055 pygpt_net-2.2.1/src/pygpt_net/provider/loaders/web_github_issues.py
--rw-r--r--   0        0        0     4377 2024-04-17 01:35:30.426055 pygpt_net-2.2.1/src/pygpt_net/provider/loaders/web_github_repo.py
--rw-r--r--   0        0        0     2834 2024-04-17 01:35:30.430055 pygpt_net-2.2.1/src/pygpt_net/provider/loaders/web_google_calendar.py
--rw-r--r--   0        0        0     2480 2024-04-17 01:35:30.430055 pygpt_net-2.2.1/src/pygpt_net/provider/loaders/web_google_docs.py
--rw-r--r--   0        0        0     3582 2024-04-17 01:35:30.430055 pygpt_net-2.2.1/src/pygpt_net/provider/loaders/web_google_drive.py
--rw-r--r--   0        0        0     2710 2024-04-17 01:35:30.430055 pygpt_net-2.2.1/src/pygpt_net/provider/loaders/web_google_gmail.py
--rw-r--r--   0        0        0     2412 2024-04-17 01:35:30.430055 pygpt_net-2.2.1/src/pygpt_net/provider/loaders/web_google_keep.py
--rw-r--r--   0        0        0     2590 2024-04-17 01:35:30.430055 pygpt_net-2.2.1/src/pygpt_net/provider/loaders/web_google_sheets.py
--rw-r--r--   0        0        0     4004 2024-04-17 01:35:30.430055 pygpt_net-2.2.1/src/pygpt_net/provider/loaders/web_microsoft_onedrive.py
--rw-r--r--   0        0        0     1572 2024-03-12 06:49:17.168786 pygpt_net-2.2.1/src/pygpt_net/provider/loaders/web_page.py
--rw-r--r--   0        0        0     1584 2024-03-12 06:49:17.172787 pygpt_net-2.2.1/src/pygpt_net/provider/loaders/web_rss.py
--rw-r--r--   0        0        0     1853 2024-04-17 01:35:30.430055 pygpt_net-2.2.1/src/pygpt_net/provider/loaders/web_sitemap.py
--rw-r--r--   0        0        0     2831 2024-04-17 01:35:30.430055 pygpt_net-2.2.1/src/pygpt_net/provider/loaders/web_twitter.py
--rw-r--r--   0        0        0     1617 2024-03-12 06:49:17.172787 pygpt_net-2.2.1/src/pygpt_net/provider/loaders/web_yt.py
--rw-r--r--   0        0        0     5976 2024-03-08 22:55:56.889343 pygpt_net-2.2.1/src/pygpt_net/provider/vector_stores/__init__.py
--rw-r--r--   0        0        0     3791 2024-03-11 03:15:21.875594 pygpt_net-2.2.1/src/pygpt_net/provider/vector_stores/base.py
--rwxr-xr-x   0        0        0     3036 2024-03-11 03:15:21.875594 pygpt_net-2.2.1/src/pygpt_net/provider/vector_stores/chroma.py
--rw-r--r--   0        0        0     3016 2024-03-11 03:15:21.875594 pygpt_net-2.2.1/src/pygpt_net/provider/vector_stores/elasticsearch.py
--rw-r--r--   0        0        0     5041 2024-03-11 03:15:21.875594 pygpt_net-2.2.1/src/pygpt_net/provider/vector_stores/pinecode.py
--rw-r--r--   0        0        0     3047 2024-03-11 03:15:21.875594 pygpt_net-2.2.1/src/pygpt_net/provider/vector_stores/redis.py
--rw-r--r--   0        0        0     2455 2024-03-11 03:15:21.875594 pygpt_net-2.2.1/src/pygpt_net/provider/vector_stores/simple.py
--rw-r--r--   0        0        0     4322 2024-03-11 03:15:21.875594 pygpt_net-2.2.1/src/pygpt_net/provider/vector_stores/temp.py
--rw-r--r--   0        0        0      488 2024-02-24 01:55:58.449111 pygpt_net-2.2.1/src/pygpt_net/provider/web/__init__.py
--rw-r--r--   0        0        0     1994 2024-02-27 05:21:39.771084 pygpt_net-2.2.1/src/pygpt_net/provider/web/base.py
--rw-r--r--   0        0        0     4646 2024-02-25 00:27:02.862945 pygpt_net-2.2.1/src/pygpt_net/provider/web/google_custom_search.py
--rw-r--r--   0        0        0     4104 2024-02-25 00:27:02.862945 pygpt_net-2.2.1/src/pygpt_net/provider/web/microsoft_bing.py
--rw-r--r--   0        0        0     3917 2024-04-19 00:32:20.498428 pygpt_net-2.2.1/src/pygpt_net/tools/__init__.py
--rwxr-xr-x   0        0        0     9791 2024-03-26 17:12:51.294309 pygpt_net-2.2.1/src/pygpt_net/tools/audio_transcriber/__init__.py
--rw-r--r--   0        0        0        0 2024-03-26 17:12:51.294309 pygpt_net-2.2.1/src/pygpt_net/tools/audio_transcriber/ui/__init__.py
--rw-r--r--   0        0        0     5666 2024-03-26 17:12:51.294309 pygpt_net-2.2.1/src/pygpt_net/tools/audio_transcriber/ui/dialogs.py
--rw-r--r--   0        0        0     2116 2024-04-19 00:32:20.498428 pygpt_net-2.2.1/src/pygpt_net/tools/base.py
--rwxr-xr-x   0        0        0    11427 2024-04-19 00:32:20.498428 pygpt_net-2.2.1/src/pygpt_net/tools/code_interpreter/__init__.py
--rw-r--r--   0        0        0        0 2024-03-26 17:12:51.294309 pygpt_net-2.2.1/src/pygpt_net/tools/code_interpreter/ui/__init__.py
--rw-r--r--   0        0        0     6580 2024-03-26 17:12:51.294309 pygpt_net-2.2.1/src/pygpt_net/tools/code_interpreter/ui/dialogs.py
--rw-r--r--   0        0        0     3518 2024-03-26 17:12:51.294309 pygpt_net-2.2.1/src/pygpt_net/tools/code_interpreter/ui/widgets.py
--rwxr-xr-x   0        0        0     9063 2024-04-14 16:40:07.849541 pygpt_net-2.2.1/src/pygpt_net/tools/image_viewer/__init__.py
--rw-r--r--   0        0        0        0 2024-03-26 17:12:51.294309 pygpt_net-2.2.1/src/pygpt_net/tools/image_viewer/ui/__init__.py
--rw-r--r--   0        0        0     4962 2024-03-26 17:12:51.294309 pygpt_net-2.2.1/src/pygpt_net/tools/image_viewer/ui/dialogs.py
--rwxr-xr-x   0        0        0    18833 2024-04-19 00:32:20.498428 pygpt_net-2.2.1/src/pygpt_net/tools/indexer/__init__.py
--rw-r--r--   0        0        0        0 2024-04-17 01:35:30.430055 pygpt_net-2.2.1/src/pygpt_net/tools/indexer/ui/__init__.py
--rw-r--r--   0        0        0     1438 2024-04-17 01:35:30.430055 pygpt_net-2.2.1/src/pygpt_net/tools/indexer/ui/browse.py
--rw-r--r--   0        0        0     4355 2024-04-17 01:35:30.430055 pygpt_net-2.2.1/src/pygpt_net/tools/indexer/ui/ctx.py
--rw-r--r--   0        0        0     7985 2024-04-17 01:35:30.430055 pygpt_net-2.2.1/src/pygpt_net/tools/indexer/ui/dialogs.py
--rw-r--r--   0        0        0     4034 2024-04-17 01:35:30.430055 pygpt_net-2.2.1/src/pygpt_net/tools/indexer/ui/files.py
--rw-r--r--   0        0        0    10477 2024-04-17 01:35:30.430055 pygpt_net-2.2.1/src/pygpt_net/tools/indexer/ui/web.py
--rw-r--r--   0        0        0     3562 2024-04-17 01:35:30.430055 pygpt_net-2.2.1/src/pygpt_net/tools/indexer/ui/widgets.py
--rwxr-xr-x   0        0        0     6028 2024-03-26 17:12:51.294309 pygpt_net-2.2.1/src/pygpt_net/tools/media_player/__init__.py
--rw-r--r--   0        0        0        0 2024-03-26 17:12:51.294309 pygpt_net-2.2.1/src/pygpt_net/tools/media_player/ui/__init__.py
--rw-r--r--   0        0        0     3590 2024-03-26 17:12:51.294309 pygpt_net-2.2.1/src/pygpt_net/tools/media_player/ui/dialogs.py
--rw-r--r--   0        0        0    15702 2024-03-26 17:12:51.294309 pygpt_net-2.2.1/src/pygpt_net/tools/media_player/ui/widgets.py
--rw-r--r--   0        0        0     8018 2024-04-14 16:40:07.849541 pygpt_net-2.2.1/src/pygpt_net/tools/text_editor/__init__.py
--rw-r--r--   0        0        0        0 2024-03-26 17:12:51.294309 pygpt_net-2.2.1/src/pygpt_net/tools/text_editor/ui/__init__.py
--rw-r--r--   0        0        0     2906 2024-04-11 00:43:06.922864 pygpt_net-2.2.1/src/pygpt_net/tools/text_editor/ui/dialogs.py
--rw-r--r--   0        0        0     2754 2024-04-11 03:43:59.058733 pygpt_net-2.2.1/src/pygpt_net/tools/text_editor/ui/widgets.py
--rwxr-xr-x   0        0        0     6639 2024-04-10 01:07:30.188635 pygpt_net-2.2.1/src/pygpt_net/ui/__init__.py
--rw-r--r--   0        0        0        0 2024-01-08 20:36:28.054492 pygpt_net-2.2.1/src/pygpt_net/ui/base/__init__.py
--rw-r--r--   0        0        0     9209 2024-03-11 07:32:25.337990 pygpt_net-2.2.1/src/pygpt_net/ui/base/config_dialog.py
--rw-r--r--   0        0        0     3430 2024-03-26 17:12:51.294309 pygpt_net-2.2.1/src/pygpt_net/ui/base/context_menu.py
--rwxr-xr-x   0        0        0      488 2023-12-28 18:11:19.000000 pygpt_net-2.2.1/src/pygpt_net/ui/dialog/__init__.py
--rwxr-xr-x   0        0        0     5730 2024-04-11 20:50:24.193030 pygpt_net-2.2.1/src/pygpt_net/ui/dialog/about.py
--rwxr-xr-x   0        0        0     5140 2024-03-26 17:12:51.294309 pygpt_net-2.2.1/src/pygpt_net/ui/dialog/applog.py
--rwxr-xr-x   0        0        0     6480 2024-04-28 06:16:26.324027 pygpt_net-2.2.1/src/pygpt_net/ui/dialog/assistant.py
--rw-r--r--   0        0        0    17707 2024-04-27 07:58:32.754704 pygpt_net-2.2.1/src/pygpt_net/ui/dialog/assistant_store.py
--rwxr-xr-x   0        0        0     1765 2024-03-18 02:45:45.661442 pygpt_net-2.2.1/src/pygpt_net/ui/dialog/changelog.py
--rw-r--r--   0        0        0      973 2024-01-28 19:32:28.495073 pygpt_net-2.2.1/src/pygpt_net/ui/dialog/create.py
--rw-r--r--   0        0        0    18520 2024-04-17 01:35:30.430055 pygpt_net-2.2.1/src/pygpt_net/ui/dialog/db.py
--rwxr-xr-x   0        0        0     1864 2024-03-18 04:54:07.637826 pygpt_net-2.2.1/src/pygpt_net/ui/dialog/debug.py
--rw-r--r--   0        0        0     5835 2024-03-12 06:49:17.172787 pygpt_net-2.2.1/src/pygpt_net/ui/dialog/dictionary.py
--rwxr-xr-x   0        0        0     2926 2024-04-10 01:07:30.188635 pygpt_net-2.2.1/src/pygpt_net/ui/dialog/editor.py
--rw-r--r--   0        0        0      957 2024-04-08 04:19:15.433912 pygpt_net-2.2.1/src/pygpt_net/ui/dialog/find.py
--rwxr-xr-x   0        0        0     2876 2024-03-26 17:12:51.294309 pygpt_net-2.2.1/src/pygpt_net/ui/dialog/image.py
--rwxr-xr-x   0        0        0     2272 2024-03-18 02:45:42.817463 pygpt_net-2.2.1/src/pygpt_net/ui/dialog/license.py
--rwxr-xr-x   0        0        0     1823 2024-03-26 17:12:51.294309 pygpt_net-2.2.1/src/pygpt_net/ui/dialog/logger.py
--rw-r--r--   0        0        0    13166 2024-03-10 12:05:00.639613 pygpt_net-2.2.1/src/pygpt_net/ui/dialog/models.py
--rwxr-xr-x   0        0        0    20679 2024-03-12 06:49:17.172787 pygpt_net-2.2.1/src/pygpt_net/ui/dialog/plugins.py
--rwxr-xr-x   0        0        0     6644 2024-02-15 05:07:04.122540 pygpt_net-2.2.1/src/pygpt_net/ui/dialog/preset.py
--rw-r--r--   0        0        0     3796 2024-03-07 01:04:26.445956 pygpt_net-2.2.1/src/pygpt_net/ui/dialog/preset_plugins.py
--rw-r--r--   0        0        0     4105 2024-04-10 01:07:30.188635 pygpt_net-2.2.1/src/pygpt_net/ui/dialog/profile.py
--rwxr-xr-x   0        0        0      973 2024-01-28 19:32:28.495073 pygpt_net-2.2.1/src/pygpt_net/ui/dialog/rename.py
--rwxr-xr-x   0        0        0    15113 2024-03-10 12:05:00.639613 pygpt_net-2.2.1/src/pygpt_net/ui/dialog/settings.py
--rw-r--r--   0        0        0      954 2024-02-26 22:26:37.124323 pygpt_net-2.2.1/src/pygpt_net/ui/dialog/snap.py
--rwxr-xr-x   0        0        0     2436 2024-02-25 05:55:37.513980 pygpt_net-2.2.1/src/pygpt_net/ui/dialog/start.py
--rwxr-xr-x   0        0        0      842 2023-12-28 18:11:19.000000 pygpt_net-2.2.1/src/pygpt_net/ui/dialog/update.py
--rw-r--r--   0        0        0     4275 2024-03-26 17:12:51.294309 pygpt_net-2.2.1/src/pygpt_net/ui/dialog/workdir.py
--rwxr-xr-x   0        0        0     9009 2024-04-26 21:55:50.679597 pygpt_net-2.2.1/src/pygpt_net/ui/dialogs.py
--rwxr-xr-x   0        0        0      488 2023-12-28 21:20:40.362230 pygpt_net-2.2.1/src/pygpt_net/ui/layout/__init__.py
--rwxr-xr-x   0        0        0     1535 2024-04-09 20:34:52.308546 pygpt_net-2.2.1/src/pygpt_net/ui/layout/chat/__init__.py
--rwxr-xr-x   0        0        0     5518 2024-04-14 20:50:29.556142 pygpt_net-2.2.1/src/pygpt_net/ui/layout/chat/attachments.py
--rwxr-xr-x   0        0        0     5356 2024-04-27 07:58:32.754704 pygpt_net-2.2.1/src/pygpt_net/ui/layout/chat/attachments_uploaded.py
--rw-r--r--   0        0        0     5996 2024-04-10 01:07:30.188635 pygpt_net-2.2.1/src/pygpt_net/ui/layout/chat/calendar.py
--rwxr-xr-x   0        0        0     9885 2024-04-09 20:35:55.668463 pygpt_net-2.2.1/src/pygpt_net/ui/layout/chat/input.py
--rwxr-xr-x   0        0        0    18656 2024-01-01 00:17:57.553256 pygpt_net-2.2.1/src/pygpt_net/ui/layout/chat/markdown.py
--rwxr-xr-x   0        0        0    10452 2024-04-21 18:06:27.128064 pygpt_net-2.2.1/src/pygpt_net/ui/layout/chat/output.py
--rw-r--r--   0        0        0     5199 2024-02-17 21:22:47.345663 pygpt_net-2.2.1/src/pygpt_net/ui/layout/chat/painter.py
--rwxr-xr-x   0        0        0     1697 2024-01-27 21:42:30.964980 pygpt_net-2.2.1/src/pygpt_net/ui/layout/ctx/__init__.py
--rwxr-xr-x   0        0        0     6648 2024-04-21 19:42:04.971470 pygpt_net-2.2.1/src/pygpt_net/ui/layout/ctx/ctx_list.py
--rwxr-xr-x   0        0        0     1441 2024-01-07 09:35:02.638810 pygpt_net-2.2.1/src/pygpt_net/ui/layout/ctx/search_input.py
--rwxr-xr-x   0        0        0     1068 2023-12-31 01:26:09.880264 pygpt_net-2.2.1/src/pygpt_net/ui/layout/ctx/video.py
--rwxr-xr-x   0        0        0     1405 2024-01-31 15:19:17.742029 pygpt_net-2.2.1/src/pygpt_net/ui/layout/status.py
--rwxr-xr-x   0        0        0     3477 2024-04-27 14:05:11.727541 pygpt_net-2.2.1/src/pygpt_net/ui/layout/toolbox/__init__.py
--rw-r--r--   0        0        0     2378 2024-01-30 17:23:19.901578 pygpt_net-2.2.1/src/pygpt_net/ui/layout/toolbox/agent.py
--rwxr-xr-x   0        0        0     4427 2024-04-27 07:58:32.754704 pygpt_net-2.2.1/src/pygpt_net/ui/layout/toolbox/assistants.py
--rwxr-xr-x   0        0        0     4254 2024-02-29 03:07:51.278132 pygpt_net-2.2.1/src/pygpt_net/ui/layout/toolbox/footer.py
--rwxr-xr-x   0        0        0     2382 2024-01-21 16:42:14.672394 pygpt_net-2.2.1/src/pygpt_net/ui/layout/toolbox/image.py
--rw-r--r--   0        0        0     6999 2024-04-27 14:05:11.727541 pygpt_net-2.2.1/src/pygpt_net/ui/layout/toolbox/indexes.py
--rwxr-xr-x   0        0        0     3169 2024-02-21 03:55:24.484309 pygpt_net-2.2.1/src/pygpt_net/ui/layout/toolbox/mode.py
--rwxr-xr-x   0        0        0     3067 2024-02-21 03:55:24.484309 pygpt_net-2.2.1/src/pygpt_net/ui/layout/toolbox/model.py
--rwxr-xr-x   0        0        0     4125 2024-03-15 15:31:21.790122 pygpt_net-2.2.1/src/pygpt_net/ui/layout/toolbox/presets.py
--rwxr-xr-x   0        0        0     3242 2024-03-15 15:31:21.790122 pygpt_net-2.2.1/src/pygpt_net/ui/layout/toolbox/prompt.py
--rwxr-xr-x   0        0        0     2447 2023-12-31 01:26:09.000000 pygpt_net-2.2.1/src/pygpt_net/ui/layout/toolbox/vision.py
--rw-r--r--   0        0        0     9613 2024-04-21 01:33:54.247764 pygpt_net-2.2.1/src/pygpt_net/ui/main.py
--rw-r--r--   0        0        0     1784 2024-03-26 17:12:51.294309 pygpt_net-2.2.1/src/pygpt_net/ui/menu/__init__.py
--rw-r--r--   0        0        0     5067 2024-04-19 00:32:20.498428 pygpt_net-2.2.1/src/pygpt_net/ui/menu/about.py
--rw-r--r--   0        0        0     1655 2024-03-20 16:01:43.283339 pygpt_net-2.2.1/src/pygpt_net/ui/menu/audio.py
--rw-r--r--   0        0        0     7870 2024-04-21 01:33:54.247764 pygpt_net-2.2.1/src/pygpt_net/ui/menu/config.py
--rw-r--r--   0        0        0     5185 2024-03-07 01:04:26.445956 pygpt_net-2.2.1/src/pygpt_net/ui/menu/debug.py
--rw-r--r--   0        0        0     3356 2024-04-17 05:13:33.075416 pygpt_net-2.2.1/src/pygpt_net/ui/menu/file.py
--rw-r--r--   0        0        0      897 2024-01-27 21:42:30.964980 pygpt_net-2.2.1/src/pygpt_net/ui/menu/lang.py
--rw-r--r--   0        0        0     2880 2024-03-07 01:04:26.445956 pygpt_net-2.2.1/src/pygpt_net/ui/menu/plugins.py
--rwxr-xr-x   0        0        0     3440 2024-04-24 23:37:32.616565 pygpt_net-2.2.1/src/pygpt_net/ui/menu/theme.py
--rw-r--r--   0        0        0     1134 2024-03-26 17:12:51.298308 pygpt_net-2.2.1/src/pygpt_net/ui/menu/tools.py
--rw-r--r--   0        0        0     2026 2024-03-20 16:01:43.283339 pygpt_net-2.2.1/src/pygpt_net/ui/menu/video.py
--rw-r--r--   0        0        0     6711 2024-04-14 20:50:29.556142 pygpt_net-2.2.1/src/pygpt_net/ui/tray.py
--rwxr-xr-x   0        0        0      488 2023-12-28 18:11:19.000000 pygpt_net-2.2.1/src/pygpt_net/ui/widget/__init__.py
--rwxr-xr-x   0        0        0      488 2023-12-28 21:20:40.362230 pygpt_net-2.2.1/src/pygpt_net/ui/widget/audio/__init__.py
--rwxr-xr-x   0        0        0     1721 2023-12-28 21:20:40.362230 pygpt_net-2.2.1/src/pygpt_net/ui/widget/audio/input.py
--rw-r--r--   0        0        0     2198 2024-02-29 03:07:51.278132 pygpt_net-2.2.1/src/pygpt_net/ui/widget/audio/input_button.py
--rwxr-xr-x   0        0        0     1586 2023-12-28 21:20:40.362230 pygpt_net-2.2.1/src/pygpt_net/ui/widget/audio/output.py
--rw-r--r--   0        0        0        0 2024-01-06 03:25:04.270157 pygpt_net-2.2.1/src/pygpt_net/ui/widget/calendar/__init__.py
--rw-r--r--   0        0        0     8120 2024-04-27 07:58:32.754704 pygpt_net-2.2.1/src/pygpt_net/ui/widget/calendar/select.py
--rwxr-xr-x   0        0        0      488 2023-12-28 21:20:40.362230 pygpt_net-2.2.1/src/pygpt_net/ui/widget/dialog/__init__.py
--rwxr-xr-x   0        0        0     1429 2024-04-17 01:35:30.430055 pygpt_net-2.2.1/src/pygpt_net/ui/widget/dialog/alert.py
--rw-r--r--   0        0        0     1502 2024-02-17 21:22:47.345663 pygpt_net-2.2.1/src/pygpt_net/ui/widget/dialog/applog.py
--rw-r--r--   0        0        0     1712 2024-04-26 21:55:50.679597 pygpt_net-2.2.1/src/pygpt_net/ui/widget/dialog/assistant_store.py
--rw-r--r--   0        0        0      551 2024-03-26 17:12:51.298308 pygpt_net-2.2.1/src/pygpt_net/ui/widget/dialog/audio.py
--rwxr-xr-x   0        0        0     3802 2024-04-11 03:43:59.058733 pygpt_net-2.2.1/src/pygpt_net/ui/widget/dialog/base.py
--rwxr-xr-x   0        0        0     2302 2024-04-12 10:08:45.275113 pygpt_net-2.2.1/src/pygpt_net/ui/widget/dialog/confirm.py
--rw-r--r--   0        0        0     2191 2024-01-28 19:32:28.495073 pygpt_net-2.2.1/src/pygpt_net/ui/widget/dialog/create.py
--rw-r--r--   0        0        0     1585 2024-03-07 01:04:26.445956 pygpt_net-2.2.1/src/pygpt_net/ui/widget/dialog/db.py
--rwxr-xr-x   0        0        0     1572 2024-02-21 16:35:35.211671 pygpt_net-2.2.1/src/pygpt_net/ui/widget/dialog/debug.py
--rwxr-xr-x   0        0        0     1749 2024-02-17 21:22:47.345663 pygpt_net-2.2.1/src/pygpt_net/ui/widget/dialog/editor.py
--rwxr-xr-x   0        0        0     6185 2024-04-14 16:40:07.849541 pygpt_net-2.2.1/src/pygpt_net/ui/widget/dialog/editor_file.py
--rw-r--r--   0        0        0     3242 2024-04-11 03:43:59.058733 pygpt_net-2.2.1/src/pygpt_net/ui/widget/dialog/find.py
--rwxr-xr-x   0        0        0      816 2024-03-26 17:12:51.298308 pygpt_net-2.2.1/src/pygpt_net/ui/widget/dialog/image.py
--rwxr-xr-x   0        0        0     1568 2024-02-17 21:22:47.345663 pygpt_net-2.2.1/src/pygpt_net/ui/widget/dialog/info.py
--rw-r--r--   0        0        0     1717 2024-02-17 21:22:47.345663 pygpt_net-2.2.1/src/pygpt_net/ui/widget/dialog/license.py
--rwxr-xr-x   0        0        0     1627 2024-02-17 21:22:47.345663 pygpt_net-2.2.1/src/pygpt_net/ui/widget/dialog/logger.py
--rw-r--r--   0        0        0     1625 2024-02-17 21:22:47.345663 pygpt_net-2.2.1/src/pygpt_net/ui/widget/dialog/model.py
--rw-r--r--   0        0        0     1694 2024-04-10 01:07:30.188635 pygpt_net-2.2.1/src/pygpt_net/ui/widget/dialog/preset_plugins.py
--rw-r--r--   0        0        0     6686 2024-04-19 00:32:20.502428 pygpt_net-2.2.1/src/pygpt_net/ui/widget/dialog/profile.py
--rwxr-xr-x   0        0        0     2191 2024-01-28 19:32:28.495073 pygpt_net-2.2.1/src/pygpt_net/ui/widget/dialog/rename.py
--rwxr-xr-x   0        0        0     1614 2024-02-17 21:22:47.345663 pygpt_net-2.2.1/src/pygpt_net/ui/widget/dialog/settings.py
--rwxr-xr-x   0        0        0     1696 2024-02-17 21:22:47.345663 pygpt_net-2.2.1/src/pygpt_net/ui/widget/dialog/settings_plugin.py
--rw-r--r--   0        0        0     2724 2024-02-26 22:26:37.124323 pygpt_net-2.2.1/src/pygpt_net/ui/widget/dialog/snap.py
--rwxr-xr-x   0        0        0     6789 2024-02-17 21:22:47.345663 pygpt_net-2.2.1/src/pygpt_net/ui/widget/dialog/update.py
--rw-r--r--   0        0        0     1523 2024-03-26 17:12:51.298308 pygpt_net-2.2.1/src/pygpt_net/ui/widget/dialog/workdir.py
--rwxr-xr-x   0        0        0      488 2024-01-11 15:56:53.277343 pygpt_net-2.2.1/src/pygpt_net/ui/widget/draw/__init__.py
--rw-r--r--   0        0        0    10903 2024-04-12 07:23:35.946682 pygpt_net-2.2.1/src/pygpt_net/ui/widget/draw/painter.py
--rwxr-xr-x   0        0        0      488 2023-12-28 21:20:40.362230 pygpt_net-2.2.1/src/pygpt_net/ui/widget/element/__init__.py
--rw-r--r--   0        0        0     2854 2024-04-14 20:50:29.556142 pygpt_net-2.2.1/src/pygpt_net/ui/widget/element/button.py
--rw-r--r--   0        0        0     2532 2024-03-07 01:04:26.445956 pygpt_net-2.2.1/src/pygpt_net/ui/widget/element/checkbox.py
--rwxr-xr-x   0        0        0     2559 2024-01-27 21:42:30.964980 pygpt_net-2.2.1/src/pygpt_net/ui/widget/element/group.py
--rw-r--r--   0        0        0     3789 2024-02-28 03:58:59.313445 pygpt_net-2.2.1/src/pygpt_net/ui/widget/element/labels.py
--rwxr-xr-x   0        0        0        0 2023-12-28 21:20:40.362230 pygpt_net-2.2.1/src/pygpt_net/ui/widget/filesystem/__init__.py
--rwxr-xr-x   0        0        0    22934 2024-04-17 01:35:30.430055 pygpt_net-2.2.1/src/pygpt_net/ui/widget/filesystem/explorer.py
--rwxr-xr-x   0        0        0      488 2023-12-28 21:20:40.362230 pygpt_net-2.2.1/src/pygpt_net/ui/widget/image/__init__.py
--rwxr-xr-x   0        0        0     3797 2024-03-26 17:12:51.298308 pygpt_net-2.2.1/src/pygpt_net/ui/widget/image/display.py
--rwxr-xr-x   0        0        0      488 2023-12-28 21:20:40.362230 pygpt_net-2.2.1/src/pygpt_net/ui/widget/lists/__init__.py
--rwxr-xr-x   0        0        0     2682 2024-01-29 13:41:53.379769 pygpt_net-2.2.1/src/pygpt_net/ui/widget/lists/assistant.py
--rw-r--r--   0        0        0     1956 2024-04-26 21:55:50.679597 pygpt_net-2.2.1/src/pygpt_net/ui/widget/lists/assistant_store.py
--rwxr-xr-x   0        0        0     7055 2024-04-14 20:50:29.556142 pygpt_net-2.2.1/src/pygpt_net/ui/widget/lists/attachment.py
--rwxr-xr-x   0        0        0     2446 2024-04-10 01:07:30.188635 pygpt_net-2.2.1/src/pygpt_net/ui/widget/lists/base.py
--rwxr-xr-x   0        0        0    17502 2024-04-17 01:35:30.430055 pygpt_net-2.2.1/src/pygpt_net/ui/widget/lists/context.py
--rw-r--r--   0        0        0     5861 2024-04-17 01:35:30.430055 pygpt_net-2.2.1/src/pygpt_net/ui/widget/lists/db.py
--rw-r--r--   0        0        0     3658 2024-03-07 01:04:26.449956 pygpt_net-2.2.1/src/pygpt_net/ui/widget/lists/debug.py
--rw-r--r--   0        0        0     4818 2024-04-17 01:35:30.430055 pygpt_net-2.2.1/src/pygpt_net/ui/widget/lists/index.py
--rw-r--r--   0        0        0     6794 2024-04-27 14:05:11.727541 pygpt_net-2.2.1/src/pygpt_net/ui/widget/lists/index_combo.py
--rwxr-xr-x   0        0        0     1080 2023-12-28 21:20:40.362230 pygpt_net-2.2.1/src/pygpt_net/ui/widget/lists/mode.py
--rwxr-xr-x   0        0        0     1912 2024-01-29 13:41:53.379769 pygpt_net-2.2.1/src/pygpt_net/ui/widget/lists/model.py
--rw-r--r--   0        0        0     1919 2024-01-29 13:41:53.379769 pygpt_net-2.2.1/src/pygpt_net/ui/widget/lists/model_editor.py
--rwxr-xr-x   0        0        0     1028 2024-01-12 09:25:47.589375 pygpt_net-2.2.1/src/pygpt_net/ui/widget/lists/plugin.py
--rwxr-xr-x   0        0        0     4071 2024-02-01 01:48:09.378583 pygpt_net-2.2.1/src/pygpt_net/ui/widget/lists/preset.py
--rw-r--r--   0        0        0     3899 2024-03-07 01:04:26.449956 pygpt_net-2.2.1/src/pygpt_net/ui/widget/lists/preset_plugins.py
--rw-r--r--   0        0        0     4432 2024-04-10 01:07:30.192635 pygpt_net-2.2.1/src/pygpt_net/ui/widget/lists/profile.py
--rw-r--r--   0        0        0     1052 2024-01-12 09:25:47.589375 pygpt_net-2.2.1/src/pygpt_net/ui/widget/lists/settings.py
--rwxr-xr-x   0        0        0     4382 2024-04-26 21:55:50.679597 pygpt_net-2.2.1/src/pygpt_net/ui/widget/lists/uploaded.py
--rwxr-xr-x   0        0        0      488 2023-12-28 21:20:40.362230 pygpt_net-2.2.1/src/pygpt_net/ui/widget/option/__init__.py
--rwxr-xr-x   0        0        0     2068 2024-01-19 21:21:41.774598 pygpt_net-2.2.1/src/pygpt_net/ui/widget/option/checkbox.py
--rw-r--r--   0        0        0     5503 2024-03-12 06:49:17.172787 pygpt_net-2.2.1/src/pygpt_net/ui/widget/option/cmd.py
--rw-r--r--   0        0        0     3592 2024-04-27 10:44:46.049374 pygpt_net-2.2.1/src/pygpt_net/ui/widget/option/combo.py
--rwxr-xr-x   0        0        0    12672 2024-03-11 03:15:21.879593 pygpt_net-2.2.1/src/pygpt_net/ui/widget/option/dictionary.py
--rwxr-xr-x   0        0        0     9304 2024-04-26 21:55:50.679597 pygpt_net-2.2.1/src/pygpt_net/ui/widget/option/input.py
--rw-r--r--   0        0        0     2601 2024-04-22 22:35:26.800429 pygpt_net-2.2.1/src/pygpt_net/ui/widget/option/prompt.py
--rwxr-xr-x   0        0        0     3569 2024-01-08 20:36:28.058493 pygpt_net-2.2.1/src/pygpt_net/ui/widget/option/slider.py
--rwxr-xr-x   0        0        0     2684 2024-04-26 21:55:50.679597 pygpt_net-2.2.1/src/pygpt_net/ui/widget/option/textarea.py
--rw-r--r--   0        0        0     1668 2024-01-29 13:41:53.379769 pygpt_net-2.2.1/src/pygpt_net/ui/widget/tabs/Input.py
--rw-r--r--   0        0        0      488 2023-12-30 09:04:29.205425 pygpt_net-2.2.1/src/pygpt_net/ui/widget/tabs/__init__.py
--rw-r--r--   0        0        0     2814 2024-04-10 01:07:30.192635 pygpt_net-2.2.1/src/pygpt_net/ui/widget/tabs/output.py
--rwxr-xr-x   0        0        0      488 2023-12-28 21:20:40.366230 pygpt_net-2.2.1/src/pygpt_net/ui/widget/textarea/__init__.py
--rw-r--r--   0        0        0     5098 2024-04-21 01:33:54.247764 pygpt_net-2.2.1/src/pygpt_net/ui/widget/textarea/calendar_note.py
--rw-r--r--   0        0        0     1358 2024-01-28 19:32:28.495073 pygpt_net-2.2.1/src/pygpt_net/ui/widget/textarea/create.py
--rw-r--r--   0        0        0     5450 2024-04-21 01:33:54.247764 pygpt_net-2.2.1/src/pygpt_net/ui/widget/textarea/editor.py
--rw-r--r--   0        0        0     1543 2024-04-11 03:43:59.058733 pygpt_net-2.2.1/src/pygpt_net/ui/widget/textarea/find.py
--rwxr-xr-x   0        0        0     6059 2024-04-22 22:35:26.800429 pygpt_net-2.2.1/src/pygpt_net/ui/widget/textarea/input.py
--rwxr-xr-x   0        0        0     1132 2024-01-27 21:42:30.964980 pygpt_net-2.2.1/src/pygpt_net/ui/widget/textarea/name.py
--rwxr-xr-x   0        0        0     6583 2024-04-21 01:33:54.247764 pygpt_net-2.2.1/src/pygpt_net/ui/widget/textarea/notepad.py
--rwxr-xr-x   0        0        0     5086 2024-04-23 23:11:13.260159 pygpt_net-2.2.1/src/pygpt_net/ui/widget/textarea/output.py
--rwxr-xr-x   0        0        0     1358 2024-01-28 19:32:28.495073 pygpt_net-2.2.1/src/pygpt_net/ui/widget/textarea/rename.py
--rwxr-xr-x   0        0        0     1833 2024-04-12 10:08:45.275113 pygpt_net-2.2.1/src/pygpt_net/ui/widget/textarea/search_input.py
--rwxr-xr-x   0        0        0    10060 2024-04-27 14:05:11.727541 pygpt_net-2.2.1/src/pygpt_net/ui/widget/textarea/web.py
--rwxr-xr-x   0        0        0      488 2023-12-28 21:20:40.366230 pygpt_net-2.2.1/src/pygpt_net/ui/widget/vision/__init__.py
--rwxr-xr-x   0        0        0     2584 2023-12-28 21:20:40.366230 pygpt_net-2.2.1/src/pygpt_net/ui/widget/vision/camera.py
--rwxr-xr-x   0        0        0     5470 2024-04-26 21:55:50.679597 pygpt_net-2.2.1/src/pygpt_net/utils.py
--rw-r--r--   0        0        0   135202 1970-01-01 00:00:00.000000 pygpt_net-2.2.1/PKG-INFO
+-rwxr-xr-x   0        0        0    57775 2024-04-29 05:51:11.628212 pygpt_net-2.2.2/CHANGELOG.md
+-rwxr-xr-x   0        0        0     1077 2024-02-01 17:53:56.362106 pygpt_net-2.2.2/LICENSE
+-rwxr-xr-x   0        0        0   131993 2024-04-29 05:51:11.628212 pygpt_net-2.2.2/README.md
+-rwxr-xr-x   0        0        0    13970 2024-02-19 21:38:20.920806 pygpt_net-2.2.2/icon.png
+-rw-r--r--   0        0        0     2979 2024-04-29 05:51:11.636212 pygpt_net-2.2.2/pyproject.toml
+-rwxr-xr-x   0        0        0    56755 2024-04-29 05:51:11.636212 pygpt_net-2.2.2/src/pygpt_net/CHANGELOG.txt
+-rwxr-xr-x   0        0        0     1146 2024-02-01 17:53:56.366106 pygpt_net-2.2.2/src/pygpt_net/LICENSE
+-rwxr-xr-x   0        0        0     1024 2024-04-29 05:51:11.636212 pygpt_net-2.2.2/src/pygpt_net/__init__.py
+-rwxr-xr-x   0        0        0    14345 2024-04-17 01:35:30.422055 pygpt_net-2.2.2/src/pygpt_net/app.py
+-rwxr-xr-x   0        0        0    15484 2024-04-29 05:51:11.636212 pygpt_net-2.2.2/src/pygpt_net/config.py
+-rwxr-xr-x   0        0        0     3601 2024-04-29 05:51:11.636212 pygpt_net-2.2.2/src/pygpt_net/container.py
+-rwxr-xr-x   0        0        0     5164 2024-04-29 05:51:11.636212 pygpt_net-2.2.2/src/pygpt_net/controller/__init__.py
+-rw-r--r--   0        0        0     4662 2024-02-25 05:32:34.229344 pygpt_net-2.2.2/src/pygpt_net/controller/agent/__init__.py
+-rw-r--r--   0        0        0     6829 2024-03-17 13:18:45.622350 pygpt_net-2.2.2/src/pygpt_net/controller/agent/flow.py
+-rw-r--r--   0        0        0     9877 2024-04-29 05:51:11.636212 pygpt_net-2.2.2/src/pygpt_net/controller/assistant/__init__.py
+-rw-r--r--   0        0        0    12703 2024-04-27 07:58:32.750704 pygpt_net-2.2.2/src/pygpt_net/controller/assistant/batch.py
+-rw-r--r--   0        0        0    13203 2024-04-27 14:05:11.727541 pygpt_net-2.2.2/src/pygpt_net/controller/assistant/editor.py
+-rw-r--r--   0        0        0    14001 2024-04-27 07:58:32.750704 pygpt_net-2.2.2/src/pygpt_net/controller/assistant/files.py
+-rwxr-xr-x   0        0        0    14251 2024-04-27 14:05:11.727541 pygpt_net-2.2.2/src/pygpt_net/controller/assistant/store.py
+-rw-r--r--   0        0        0    17631 2024-04-29 05:51:11.636212 pygpt_net-2.2.2/src/pygpt_net/controller/assistant/threads.py
+-rwxr-xr-x   0        0        0    15540 2024-04-29 05:51:11.636212 pygpt_net-2.2.2/src/pygpt_net/controller/attachment.py
+-rw-r--r--   0        0        0     5972 2024-03-20 16:01:43.275339 pygpt_net-2.2.2/src/pygpt_net/controller/audio/__init__.py
+-rw-r--r--   0        0        0     3922 2024-04-29 05:51:11.636212 pygpt_net-2.2.2/src/pygpt_net/controller/calendar/__init__.py
+-rw-r--r--   0        0        0     8585 2024-04-11 03:43:59.058733 pygpt_net-2.2.2/src/pygpt_net/controller/calendar/note.py
+-rwxr-xr-x   0        0        0    12774 2024-03-15 15:31:21.786121 pygpt_net-2.2.2/src/pygpt_net/controller/camera.py
+-rw-r--r--   0        0        0     1628 2024-04-29 05:51:11.636212 pygpt_net-2.2.2/src/pygpt_net/controller/chat/__init__.py
+-rwxr-xr-x   0        0        0    11529 2024-04-29 05:51:11.636212 pygpt_net-2.2.2/src/pygpt_net/controller/chat/common.py
+-rw-r--r--   0        0        0     2144 2024-03-15 15:31:21.786121 pygpt_net-2.2.2/src/pygpt_net/controller/chat/files.py
+-rwxr-xr-x   0        0        0     6279 2024-03-26 17:12:51.286309 pygpt_net-2.2.2/src/pygpt_net/controller/chat/image.py
+-rwxr-xr-x   0        0        0     9801 2024-04-29 02:23:54.221168 pygpt_net-2.2.2/src/pygpt_net/controller/chat/input.py
+-rwxr-xr-x   0        0        0    10189 2024-04-26 21:55:50.675598 pygpt_net-2.2.2/src/pygpt_net/controller/chat/output.py
+-rwxr-xr-x   0        0        0     9610 2024-04-25 00:06:58.371551 pygpt_net-2.2.2/src/pygpt_net/controller/chat/render.py
+-rw-r--r--   0        0        0    12003 2024-04-28 06:16:26.324027 pygpt_net-2.2.2/src/pygpt_net/controller/chat/text.py
+-rw-r--r--   0        0        0     3382 2024-04-11 20:50:24.189030 pygpt_net-2.2.2/src/pygpt_net/controller/chat/vision.py
+-rw-r--r--   0        0        0     5292 2024-03-26 17:12:51.286309 pygpt_net-2.2.2/src/pygpt_net/controller/command.py
+-rw-r--r--   0        0        0     4485 2024-04-26 21:55:50.675598 pygpt_net-2.2.2/src/pygpt_net/controller/config/__init__.py
+-rw-r--r--   0        0        0        0 2024-01-08 20:36:28.054492 pygpt_net-2.2.2/src/pygpt_net/controller/config/field/__init__.py
+-rwxr-xr-x   0        0        0     2422 2024-01-30 20:56:32.772879 pygpt_net-2.2.2/src/pygpt_net/controller/config/field/checkbox.py
+-rw-r--r--   0        0        0     4863 2024-03-12 06:49:17.164785 pygpt_net-2.2.2/src/pygpt_net/controller/config/field/cmd.py
+-rw-r--r--   0        0        0     3237 2024-04-27 14:05:11.727541 pygpt_net-2.2.2/src/pygpt_net/controller/config/field/combo.py
+-rw-r--r--   0        0        0     6657 2024-03-12 06:49:17.164785 pygpt_net-2.2.2/src/pygpt_net/controller/config/field/dictionary.py
+-rw-r--r--   0        0        0     3556 2024-03-15 15:31:21.786121 pygpt_net-2.2.2/src/pygpt_net/controller/config/field/input.py
+-rw-r--r--   0        0        0     4580 2024-04-21 01:33:54.239765 pygpt_net-2.2.2/src/pygpt_net/controller/config/field/slider.py
+-rw-r--r--   0        0        0     2337 2024-04-22 21:31:19.988317 pygpt_net-2.2.2/src/pygpt_net/controller/config/field/textarea.py
+-rw-r--r--   0        0        0     7245 2024-04-24 02:39:32.054775 pygpt_net-2.2.2/src/pygpt_net/controller/config/placeholder.py
+-rw-r--r--   0        0        0    29541 2024-04-29 05:51:11.636212 pygpt_net-2.2.2/src/pygpt_net/controller/ctx/__init__.py
+-rw-r--r--   0        0        0     5434 2024-04-10 01:07:30.184635 pygpt_net-2.2.2/src/pygpt_net/controller/ctx/common.py
+-rwxr-xr-x   0        0        0     7477 2024-04-29 04:57:38.321533 pygpt_net-2.2.2/src/pygpt_net/controller/ctx/extra.py
+-rw-r--r--   0        0        0     2552 2024-01-25 22:43:11.543975 pygpt_net-2.2.2/src/pygpt_net/controller/ctx/summarizer.py
+-rw-r--r--   0        0        0     7732 2024-04-29 05:51:11.640212 pygpt_net-2.2.2/src/pygpt_net/controller/debug/__init__.py
+-rw-r--r--   0        0        0     1008 2023-12-31 03:09:04.107766 pygpt_net-2.2.2/src/pygpt_net/controller/dialogs/__init__.py
+-rwxr-xr-x   0        0        0    12973 2024-04-27 07:58:32.750704 pygpt_net-2.2.2/src/pygpt_net/controller/dialogs/confirm.py
+-rw-r--r--   0        0        0     5634 2024-03-07 01:04:26.437955 pygpt_net-2.2.2/src/pygpt_net/controller/dialogs/debug.py
+-rwxr-xr-x   0        0        0     2582 2024-04-19 00:32:20.498428 pygpt_net-2.2.2/src/pygpt_net/controller/dialogs/info.py
+-rwxr-xr-x   0        0        0    15668 2024-04-29 05:51:11.640212 pygpt_net-2.2.2/src/pygpt_net/controller/files.py
+-rwxr-xr-x   0        0        0     4874 2024-04-21 01:33:54.239765 pygpt_net-2.2.2/src/pygpt_net/controller/finder.py
+-rwxr-xr-x   0        0        0     7090 2024-04-29 05:51:11.640212 pygpt_net-2.2.2/src/pygpt_net/controller/idx/__init__.py
+-rw-r--r--   0        0        0     2605 2024-02-29 03:07:51.274132 pygpt_net-2.2.2/src/pygpt_net/controller/idx/common.py
+-rwxr-xr-x   0        0        0    21150 2024-04-17 04:14:11.980074 pygpt_net-2.2.2/src/pygpt_net/controller/idx/indexer.py
+-rw-r--r--   0        0        0     7789 2024-03-03 03:52:54.350656 pygpt_net-2.2.2/src/pygpt_net/controller/idx/settings.py
+-rw-r--r--   0        0        0     3289 2024-04-29 05:51:11.640212 pygpt_net-2.2.2/src/pygpt_net/controller/lang/__init__.py
+-rw-r--r--   0        0        0     5080 2024-04-27 14:05:11.727541 pygpt_net-2.2.2/src/pygpt_net/controller/lang/custom.py
+-rw-r--r--   0        0        0    19922 2024-04-27 14:05:11.727541 pygpt_net-2.2.2/src/pygpt_net/controller/lang/mapping.py
+-rw-r--r--   0        0        0     3879 2024-01-15 13:47:55.919633 pygpt_net-2.2.2/src/pygpt_net/controller/lang/plugins.py
+-rw-r--r--   0        0        0     2634 2024-01-22 12:10:21.917245 pygpt_net-2.2.2/src/pygpt_net/controller/lang/settings.py
+-rwxr-xr-x   0        0        0     1566 2024-01-04 07:51:17.999390 pygpt_net-2.2.2/src/pygpt_net/controller/launcher.py
+-rwxr-xr-x   0        0        0    11297 2024-04-29 05:51:11.640212 pygpt_net-2.2.2/src/pygpt_net/controller/layout.py
+-rw-r--r--   0        0        0     6521 2024-04-29 05:51:11.640212 pygpt_net-2.2.2/src/pygpt_net/controller/mode.py
+-rw-r--r--   0        0        0     4656 2024-01-30 20:56:32.772879 pygpt_net-2.2.2/src/pygpt_net/controller/model/__init__.py
+-rw-r--r--   0        0        0    12599 2024-02-22 03:36:30.096422 pygpt_net-2.2.2/src/pygpt_net/controller/model/editor.py
+-rwxr-xr-x   0        0        0    11795 2024-04-29 05:51:11.640212 pygpt_net-2.2.2/src/pygpt_net/controller/notepad.py
+-rw-r--r--   0        0        0     2572 2024-04-29 05:51:11.640212 pygpt_net-2.2.2/src/pygpt_net/controller/painter/__init__.py
+-rw-r--r--   0        0        0     4461 2024-01-23 23:46:30.495197 pygpt_net-2.2.2/src/pygpt_net/controller/painter/capture.py
+-rw-r--r--   0        0        0     6292 2024-02-17 21:22:47.341663 pygpt_net-2.2.2/src/pygpt_net/controller/painter/common.py
+-rw-r--r--   0        0        0    14232 2024-04-29 05:51:11.640212 pygpt_net-2.2.2/src/pygpt_net/controller/plugins/__init__.py
+-rw-r--r--   0        0        0    11914 2024-03-07 01:04:26.441956 pygpt_net-2.2.2/src/pygpt_net/controller/plugins/presets.py
+-rw-r--r--   0        0        0     6040 2024-04-10 03:33:51.491189 pygpt_net-2.2.2/src/pygpt_net/controller/plugins/settings.py
+-rwxr-xr-x   0        0        0    15949 2024-04-29 05:51:11.640212 pygpt_net-2.2.2/src/pygpt_net/controller/presets/__init__.py
+-rwxr-xr-x   0        0        0    14997 2024-04-22 22:35:26.800429 pygpt_net-2.2.2/src/pygpt_net/controller/presets/editor.py
+-rw-r--r--   0        0        0     7684 2024-04-29 05:51:11.640212 pygpt_net-2.2.2/src/pygpt_net/controller/settings/__init__.py
+-rwxr-xr-x   0        0        0    14833 2024-04-24 02:39:32.054775 pygpt_net-2.2.2/src/pygpt_net/controller/settings/editor.py
+-rw-r--r--   0        0        0    20965 2024-04-29 05:51:11.640212 pygpt_net-2.2.2/src/pygpt_net/controller/settings/profile.py
+-rwxr-xr-x   0        0        0     8597 2024-04-14 16:40:07.849541 pygpt_net-2.2.2/src/pygpt_net/controller/settings/workdir.py
+-rwxr-xr-x   0        0        0     6100 2024-04-29 05:51:11.640212 pygpt_net-2.2.2/src/pygpt_net/controller/theme/__init__.py
+-rwxr-xr-x   0        0        0     5435 2024-04-11 16:41:32.664297 pygpt_net-2.2.2/src/pygpt_net/controller/theme/common.py
+-rw-r--r--   0        0        0     5085 2024-04-24 23:37:32.612565 pygpt_net-2.2.2/src/pygpt_net/controller/theme/markdown.py
+-rw-r--r--   0        0        0     4631 2024-04-24 02:39:32.054775 pygpt_net-2.2.2/src/pygpt_net/controller/theme/menu.py
+-rw-r--r--   0        0        0     5028 2024-04-24 23:37:32.612565 pygpt_net-2.2.2/src/pygpt_net/controller/theme/nodes.py
+-rw-r--r--   0        0        0     6093 2024-04-11 03:43:59.058733 pygpt_net-2.2.2/src/pygpt_net/controller/ui/__init__.py
+-rw-r--r--   0        0        0     4980 2024-04-27 14:05:11.727541 pygpt_net-2.2.2/src/pygpt_net/controller/ui/mode.py
+-rw-r--r--   0        0        0     1902 2024-01-23 23:46:30.499197 pygpt_net-2.2.2/src/pygpt_net/controller/ui/vision.py
+-rw-r--r--   0        0        0        0 2024-01-26 16:05:36.561120 pygpt_net-2.2.2/src/pygpt_net/core/__init__.py
+-rw-r--r--   0        0        0     4330 2024-04-26 21:55:50.675598 pygpt_net-2.2.2/src/pygpt_net/core/assistants/__init__.py
+-rw-r--r--   0        0        0     9275 2024-04-26 21:55:50.675598 pygpt_net-2.2.2/src/pygpt_net/core/assistants/files.py
+-rw-r--r--   0        0        0     7998 2024-04-27 14:05:11.727541 pygpt_net-2.2.2/src/pygpt_net/core/assistants/store.py
+-rwxr-xr-x   0        0        0    10240 2024-01-31 15:19:17.738030 pygpt_net-2.2.2/src/pygpt_net/core/attachments.py
+-rw-r--r--   0        0        0     2708 2024-02-24 01:55:58.445111 pygpt_net-2.2.2/src/pygpt_net/core/audio.py
+-rw-r--r--   0        0        0     4466 2024-03-15 15:31:21.786121 pygpt_net-2.2.2/src/pygpt_net/core/bridge.py
+-rw-r--r--   0        0        0     6634 2024-03-12 06:49:17.164785 pygpt_net-2.2.2/src/pygpt_net/core/calendar/__init__.py
+-rwxr-xr-x   0        0        0     4034 2024-02-21 16:18:39.952987 pygpt_net-2.2.2/src/pygpt_net/core/camera.py
+-rw-r--r--   0        0        0     3130 2024-01-27 01:08:27.560991 pygpt_net-2.2.2/src/pygpt_net/core/chain/__init__.py
+-rw-r--r--   0        0        0     4656 2024-01-27 01:08:27.560991 pygpt_net-2.2.2/src/pygpt_net/core/chain/chat.py
+-rw-r--r--   0        0        0     5089 2024-01-27 01:08:27.560991 pygpt_net-2.2.2/src/pygpt_net/core/chain/completion.py
+-rwxr-xr-x   0        0        0    10217 2024-03-17 14:26:02.923314 pygpt_net-2.2.2/src/pygpt_net/core/command.py
+-rwxr-xr-x   0        0        0    31384 2024-04-17 06:16:54.016653 pygpt_net-2.2.2/src/pygpt_net/core/ctx/__init__.py
+-rw-r--r--   0        0        0     7709 2024-02-27 05:21:39.767084 pygpt_net-2.2.2/src/pygpt_net/core/ctx/idx.py
+-rw-r--r--   0        0        0    15901 2024-04-29 05:51:11.640212 pygpt_net-2.2.2/src/pygpt_net/core/db/__init__.py
+-rw-r--r--   0        0        0     8884 2024-04-17 01:35:30.422055 pygpt_net-2.2.2/src/pygpt_net/core/db/viewer.py
+-rwxr-xr-x   0        0        0     9240 2024-03-26 17:12:51.290309 pygpt_net-2.2.2/src/pygpt_net/core/debug/__init__.py
+-rw-r--r--   0        0        0     1467 2024-02-25 18:06:16.205368 pygpt_net-2.2.2/src/pygpt_net/core/debug/agent.py
+-rwxr-xr-x   0        0        0     2532 2024-04-26 21:55:50.675598 pygpt_net-2.2.2/src/pygpt_net/core/debug/assistants.py
+-rwxr-xr-x   0        0        0     1626 2024-02-25 22:01:41.690831 pygpt_net-2.2.2/src/pygpt_net/core/debug/attachments.py
+-rwxr-xr-x   0        0        0     2305 2024-04-10 01:07:30.184635 pygpt_net-2.2.2/src/pygpt_net/core/debug/config.py
+-rwxr-xr-x   0        0        0     3543 2024-04-14 04:42:08.288289 pygpt_net-2.2.2/src/pygpt_net/core/debug/context.py
+-rw-r--r--   0        0        0      776 2024-03-07 01:04:26.441956 pygpt_net-2.2.2/src/pygpt_net/core/debug/db.py
+-rw-r--r--   0        0        0     5194 2024-03-12 06:49:17.164785 pygpt_net-2.2.2/src/pygpt_net/core/debug/indexes.py
+-rwxr-xr-x   0        0        0     1848 2024-02-25 22:01:41.690831 pygpt_net-2.2.2/src/pygpt_net/core/debug/models.py
+-rwxr-xr-x   0        0        0     1258 2024-02-25 22:01:41.690831 pygpt_net-2.2.2/src/pygpt_net/core/debug/plugins.py
+-rwxr-xr-x   0        0        0     1994 2024-02-25 22:01:41.690831 pygpt_net-2.2.2/src/pygpt_net/core/debug/presets.py
+-rwxr-xr-x   0        0        0     2666 2024-02-25 22:01:41.690831 pygpt_net-2.2.2/src/pygpt_net/core/debug/ui.py
+-rwxr-xr-x   0        0        0     9012 2024-03-26 17:12:51.290309 pygpt_net-2.2.2/src/pygpt_net/core/dispatcher.py
+-rwxr-xr-x   0        0        0    14537 2024-04-21 01:33:54.243764 pygpt_net-2.2.2/src/pygpt_net/core/filesystem/__init__.py
+-rw-r--r--   0        0        0     4074 2024-03-26 17:12:51.290309 pygpt_net-2.2.2/src/pygpt_net/core/filesystem/actions.py
+-rw-r--r--   0        0        0     4123 2024-04-22 03:13:23.727782 pygpt_net-2.2.2/src/pygpt_net/core/filesystem/editor.py
+-rw-r--r--   0        0        0     3385 2024-03-19 09:04:41.050928 pygpt_net-2.2.2/src/pygpt_net/core/filesystem/types.py
+-rw-r--r--   0        0        0     2753 2024-04-21 01:33:54.243764 pygpt_net-2.2.2/src/pygpt_net/core/filesystem/url.py
+-rwxr-xr-x   0        0        0     3092 2024-01-23 23:46:30.499197 pygpt_net-2.2.2/src/pygpt_net/core/history.py
+-rwxr-xr-x   0        0        0    17238 2024-04-17 01:35:30.422055 pygpt_net-2.2.2/src/pygpt_net/core/idx/__init__.py
+-rwxr-xr-x   0        0        0    12300 2024-04-17 01:35:30.422055 pygpt_net-2.2.2/src/pygpt_net/core/idx/chat.py
+-rw-r--r--   0        0        0     2226 2024-02-28 03:58:59.309445 pygpt_net-2.2.2/src/pygpt_net/core/idx/context.py
+-rwxr-xr-x   0        0        0    31850 2024-04-17 01:35:30.422055 pygpt_net-2.2.2/src/pygpt_net/core/idx/indexing.py
+-rw-r--r--   0        0        0     4016 2024-04-26 23:49:43.379197 pygpt_net-2.2.2/src/pygpt_net/core/idx/llm.py
+-rw-r--r--   0        0        0     5304 2024-04-17 01:35:30.422055 pygpt_net-2.2.2/src/pygpt_net/core/idx/metadata.py
+-rw-r--r--   0        0        0        0 2024-02-27 05:21:39.767084 pygpt_net-2.2.2/src/pygpt_net/core/idx/types/__init__.py
+-rw-r--r--   0        0        0     3113 2024-02-27 05:21:39.767084 pygpt_net-2.2.2/src/pygpt_net/core/idx/types/ctx.py
+-rw-r--r--   0        0        0     4722 2024-02-27 05:21:39.767084 pygpt_net-2.2.2/src/pygpt_net/core/idx/types/external.py
+-rw-r--r--   0        0        0     3733 2024-02-27 05:21:39.771084 pygpt_net-2.2.2/src/pygpt_net/core/idx/types/files.py
+-rwxr-xr-x   0        0        0     3774 2024-04-17 04:14:11.980074 pygpt_net-2.2.2/src/pygpt_net/core/idx/worker.py
+-rwxr-xr-x   0        0        0     3288 2024-03-17 13:18:45.634349 pygpt_net-2.2.2/src/pygpt_net/core/image.py
+-rwxr-xr-x   0        0        0      829 2023-12-31 03:18:56.426282 pygpt_net-2.2.2/src/pygpt_net/core/info.py
+-rw-r--r--   0        0        0     2040 2024-03-25 10:26:39.426403 pygpt_net-2.2.2/src/pygpt_net/core/installer.py
+-rw-r--r--   0        0        0     1168 2024-01-14 15:51:20.622630 pygpt_net-2.2.2/src/pygpt_net/core/llm/__init__.py
+-rwxr-xr-x   0        0        0     5112 2024-04-11 16:41:32.664297 pygpt_net-2.2.2/src/pygpt_net/core/locale.py
+-rw-r--r--   0        0        0     7573 2024-01-27 21:42:30.960980 pygpt_net-2.2.2/src/pygpt_net/core/models.py
+-rw-r--r--   0        0        0     1913 2024-01-23 23:46:30.499197 pygpt_net-2.2.2/src/pygpt_net/core/modes.py
+-rwxr-xr-x   0        0        0     3378 2024-04-10 01:07:30.184635 pygpt_net-2.2.2/src/pygpt_net/core/notepad.py
+-rwxr-xr-x   0        0        0     4395 2024-03-09 21:41:28.185853 pygpt_net-2.2.2/src/pygpt_net/core/platforms.py
+-rwxr-xr-x   0        0        0    14828 2024-04-28 08:05:35.578680 pygpt_net-2.2.2/src/pygpt_net/core/plugins.py
+-rw-r--r--   0        0        0     9279 2024-03-17 13:18:45.634349 pygpt_net-2.2.2/src/pygpt_net/core/presets.py
+-rw-r--r--   0        0        0     7650 2024-04-10 01:07:30.184635 pygpt_net-2.2.2/src/pygpt_net/core/profile.py
+-rw-r--r--   0        0        0     2427 2024-04-22 22:35:26.800429 pygpt_net-2.2.2/src/pygpt_net/core/prompt/__init__.py
+-rw-r--r--   0        0        0     2798 2024-04-22 22:35:26.800429 pygpt_net-2.2.2/src/pygpt_net/core/prompt/template.py
+-rw-r--r--   0        0        0      489 2024-01-05 12:12:41.797675 pygpt_net-2.2.2/src/pygpt_net/core/render/__init__.py
+-rw-r--r--   0        0        0     5024 2024-04-24 23:37:32.612565 pygpt_net-2.2.2/src/pygpt_net/core/render/base.py
+-rwxr-xr-x   0        0        0      489 2024-04-21 01:33:54.243764 pygpt_net-2.2.2/src/pygpt_net/core/render/markdown/__init__.py
+-rwxr-xr-x   0        0        0     5450 2024-04-22 05:35:04.663179 pygpt_net-2.2.2/src/pygpt_net/core/render/markdown/parser.py
+-rwxr-xr-x   0        0        0    23291 2024-04-24 23:37:32.612565 pygpt_net-2.2.2/src/pygpt_net/core/render/markdown/renderer.py
+-rw-r--r--   0        0        0      489 2024-01-05 13:07:04.262555 pygpt_net-2.2.2/src/pygpt_net/core/render/plain/__init__.py
+-rw-r--r--   0        0        0    15716 2024-04-21 01:33:54.243764 pygpt_net-2.2.2/src/pygpt_net/core/render/plain/renderer.py
+-rwxr-xr-x   0        0        0      489 2024-04-21 01:33:54.000000 pygpt_net-2.2.2/src/pygpt_net/core/render/web/__init__.py
+-rwxr-xr-x   0        0        0     8564 2024-04-28 06:16:26.324027 pygpt_net-2.2.2/src/pygpt_net/core/render/web/parser.py
+-rwxr-xr-x   0        0        0    42853 2024-04-29 05:51:11.640212 pygpt_net-2.2.2/src/pygpt_net/core/render/web/renderer.py
+-rwxr-xr-x   0        0        0     7512 2024-04-24 23:37:32.612565 pygpt_net-2.2.2/src/pygpt_net/core/settings.py
+-rw-r--r--   0        0        0        0 2024-04-21 01:33:54.243764 pygpt_net-2.2.2/src/pygpt_net/core/text/__init__.py
+-rwxr-xr-x   0        0        0     6566 2024-04-21 01:33:54.243764 pygpt_net-2.2.2/src/pygpt_net/core/text/finder.py
+-rw-r--r--   0        0        0     2250 2024-04-29 05:51:11.640212 pygpt_net-2.2.2/src/pygpt_net/core/text/utils.py
+-rw-r--r--   0        0        0     6487 2024-04-21 01:33:54.243764 pygpt_net-2.2.2/src/pygpt_net/core/text/web_finder.py
+-rwxr-xr-x   0        0        0    14040 2024-02-25 18:06:16.205368 pygpt_net-2.2.2/src/pygpt_net/core/tokens.py
+-rw-r--r--   0        0        0    13722 2024-02-21 19:09:37.240983 pygpt_net-2.2.2/src/pygpt_net/core/updater/__init__.py
+-rw-r--r--   0        0        0     2343 2024-02-24 01:55:58.445111 pygpt_net-2.2.2/src/pygpt_net/core/web.py
+-rw-r--r--   0        0        0      901 2024-01-25 22:43:11.543975 pygpt_net-2.2.2/src/pygpt_net/core/worker.py
+-rwxr-xr-x   0        0        0    10587 2024-04-29 05:51:11.640212 pygpt_net-2.2.2/src/pygpt_net/data/config/config.json
+-rwxr-xr-x   0        0        0    18526 2024-04-29 05:51:11.640212 pygpt_net-2.2.2/src/pygpt_net/data/config/models.json
+-rw-r--r--   0        0        0     1440 2024-04-29 05:51:11.640212 pygpt_net-2.2.2/src/pygpt_net/data/config/modes.json
+-rwxr-xr-x   0        0        0      459 2024-01-13 13:04:53.113674 pygpt_net-2.2.2/src/pygpt_net/data/config/presets/batman_and_joker.json
+-rw-r--r--   0        0        0     2702 2024-01-30 17:23:19.885579 pygpt_net-2.2.2/src/pygpt_net/data/config/presets/current.agent.json
+-rwxr-xr-x   0        0        0      368 2024-01-30 17:23:19.885579 pygpt_net-2.2.2/src/pygpt_net/data/config/presets/current.assistant.json
+-rwxr-xr-x   0        0        0      396 2024-01-30 17:23:19.885579 pygpt_net-2.2.2/src/pygpt_net/data/config/presets/current.chat.json
+-rwxr-xr-x   0        0        0      385 2024-01-30 17:23:19.885579 pygpt_net-2.2.2/src/pygpt_net/data/config/presets/current.completion.json
+-rwxr-xr-x   0        0        0      368 2024-01-30 17:23:19.885579 pygpt_net-2.2.2/src/pygpt_net/data/config/presets/current.img.json
+-rwxr-xr-x   0        0        0      382 2024-01-30 17:23:19.885579 pygpt_net-2.2.2/src/pygpt_net/data/config/presets/current.langchain.json
+-rw-r--r--   0        0        0      368 2024-03-03 02:59:46.037803 pygpt_net-2.2.2/src/pygpt_net/data/config/presets/current.llama_index.json
+-rwxr-xr-x   0        0        0      392 2024-03-03 03:52:54.350656 pygpt_net-2.2.2/src/pygpt_net/data/config/presets/current.vision.json
+-rwxr-xr-x   0        0        0      501 2024-01-30 17:23:19.885579 pygpt_net-2.2.2/src/pygpt_net/data/config/presets/dalle_white_cat.json
+-rwxr-xr-x   0        0        0    32497 2024-04-29 05:51:11.640212 pygpt_net-2.2.2/src/pygpt_net/data/config/settings.json
+-rw-r--r--   0        0        0      804 2024-03-17 13:18:45.634349 pygpt_net-2.2.2/src/pygpt_net/data/config/settings_section.json
+-rwxr-xr-x   0        0        0      664 2024-03-18 04:54:07.000000 pygpt_net-2.2.2/src/pygpt_net/data/css/fix_windows.css
+-rwxr-xr-x   0        0        0     1122 2024-04-19 00:29:50.000000 pygpt_net-2.2.2/src/pygpt_net/data/css/markdown.css
+-rwxr-xr-x   0        0        0      730 2024-04-19 00:29:50.000000 pygpt_net-2.2.2/src/pygpt_net/data/css/markdown.dark.css
+-rwxr-xr-x   0        0        0      833 2024-04-19 00:29:50.000000 pygpt_net-2.2.2/src/pygpt_net/data/css/markdown.light.css
+-rwxr-xr-x   0        0        0      400 2024-04-20 05:54:38.000000 pygpt_net-2.2.2/src/pygpt_net/data/css/style.css
+-rwxr-xr-x   0        0        0      729 2024-04-21 01:33:54.243764 pygpt_net-2.2.2/src/pygpt_net/data/css/style.dark.css
+-rwxr-xr-x   0        0        0     1726 2024-04-20 05:55:02.000000 pygpt_net-2.2.2/src/pygpt_net/data/css/style.light.css
+-rwxr-xr-x   0        0        0     3407 2024-04-24 23:37:32.612565 pygpt_net-2.2.2/src/pygpt_net/data/css/web.css
+-rwxr-xr-x   0        0        0     1260 2024-04-25 03:37:50.192528 pygpt_net-2.2.2/src/pygpt_net/data/css/web.dark.css
+-rwxr-xr-x   0        0        0     1235 2024-04-25 03:07:07.934949 pygpt_net-2.2.2/src/pygpt_net/data/css/web.light.css
+-rwxr-xr-x   0        0        0    69484 2023-12-08 15:03:16.000000 pygpt_net-2.2.2/src/pygpt_net/data/fonts/Lato/Lato-Black.ttf
+-rwxr-xr-x   0        0        0    71948 2023-12-08 15:03:16.000000 pygpt_net-2.2.2/src/pygpt_net/data/fonts/Lato/Lato-BlackItalic.ttf
+-rwxr-xr-x   0        0        0    73316 2023-12-08 15:03:16.000000 pygpt_net-2.2.2/src/pygpt_net/data/fonts/Lato/Lato-Bold.ttf
+-rwxr-xr-x   0        0        0    77680 2023-12-08 15:03:16.000000 pygpt_net-2.2.2/src/pygpt_net/data/fonts/Lato/Lato-BoldItalic.ttf
+-rwxr-xr-x   0        0        0    75744 2023-12-08 15:03:16.000000 pygpt_net-2.2.2/src/pygpt_net/data/fonts/Lato/Lato-Italic.ttf
+-rwxr-xr-x   0        0        0    77192 2023-12-08 15:03:16.000000 pygpt_net-2.2.2/src/pygpt_net/data/fonts/Lato/Lato-Light.ttf
+-rwxr-xr-x   0        0        0    49064 2023-12-08 15:03:16.000000 pygpt_net-2.2.2/src/pygpt_net/data/fonts/Lato/Lato-LightItalic.ttf
+-rwxr-xr-x   0        0        0    75136 2023-12-08 15:03:16.000000 pygpt_net-2.2.2/src/pygpt_net/data/fonts/Lato/Lato-Regular.ttf
+-rwxr-xr-x   0        0        0    69968 2023-12-08 15:03:16.000000 pygpt_net-2.2.2/src/pygpt_net/data/fonts/Lato/Lato-Thin.ttf
+-rwxr-xr-x   0        0        0    48848 2023-12-08 15:03:16.000000 pygpt_net-2.2.2/src/pygpt_net/data/fonts/Lato/Lato-ThinItalic.ttf
+-rwxr-xr-x   0        0        0     4500 2023-12-08 15:03:16.000000 pygpt_net-2.2.2/src/pygpt_net/data/fonts/Lato/OFL.txt
+-rw-r--r--   0        0        0    77432 2024-04-08 04:19:15.417912 pygpt_net-2.2.2/src/pygpt_net/data/fonts/MonaspaceArgon/MonaspaceArgon-Bold.otf
+-rw-r--r--   0        0        0    82112 2024-04-08 04:19:15.417912 pygpt_net-2.2.2/src/pygpt_net/data/fonts/MonaspaceArgon/MonaspaceArgon-BoldItalic.otf
+-rw-r--r--   0        0        0    81240 2024-04-08 04:19:15.417912 pygpt_net-2.2.2/src/pygpt_net/data/fonts/MonaspaceArgon/MonaspaceArgon-Italic.otf
+-rw-r--r--   0        0        0    75476 2024-04-08 04:19:15.421912 pygpt_net-2.2.2/src/pygpt_net/data/fonts/MonaspaceArgon/MonaspaceArgon-Regular.otf
+-rw-r--r--   0        0        0    75000 2024-04-08 04:19:15.421912 pygpt_net-2.2.2/src/pygpt_net/data/fonts/MonaspaceKrypton/MonaspaceKrypton-Bold.otf
+-rw-r--r--   0        0        0    77804 2024-04-08 04:19:15.421912 pygpt_net-2.2.2/src/pygpt_net/data/fonts/MonaspaceKrypton/MonaspaceKrypton-BoldItalic.otf
+-rw-r--r--   0        0        0    76752 2024-04-08 04:19:15.421912 pygpt_net-2.2.2/src/pygpt_net/data/fonts/MonaspaceKrypton/MonaspaceKrypton-Italic.otf
+-rw-r--r--   0        0        0    74248 2024-04-08 04:19:15.421912 pygpt_net-2.2.2/src/pygpt_net/data/fonts/MonaspaceKrypton/MonaspaceKrypton-Regular.otf
+-rw-r--r--   0        0        0    74120 2024-04-08 04:19:15.421912 pygpt_net-2.2.2/src/pygpt_net/data/fonts/MonaspaceNeon/MonaspaceNeon-Bold.otf
+-rw-r--r--   0        0        0    79236 2024-04-08 04:19:15.421912 pygpt_net-2.2.2/src/pygpt_net/data/fonts/MonaspaceNeon/MonaspaceNeon-BoldItalic.otf
+-rw-r--r--   0        0        0    78488 2024-04-08 04:19:15.425912 pygpt_net-2.2.2/src/pygpt_net/data/fonts/MonaspaceNeon/MonaspaceNeon-Italic.otf
+-rw-r--r--   0        0        0    73232 2024-04-08 04:19:15.425912 pygpt_net-2.2.2/src/pygpt_net/data/fonts/MonaspaceNeon/MonaspaceNeon-Regular.otf
+-rw-r--r--   0        0        0    88992 2024-04-08 04:19:15.425912 pygpt_net-2.2.2/src/pygpt_net/data/fonts/MonaspaceRadon/MonaspaceRadon-Bold.otf
+-rw-r--r--   0        0        0    94348 2024-04-08 04:19:15.425912 pygpt_net-2.2.2/src/pygpt_net/data/fonts/MonaspaceRadon/MonaspaceRadon-BoldItalic.otf
+-rw-r--r--   0        0        0    93720 2024-04-08 04:19:15.425912 pygpt_net-2.2.2/src/pygpt_net/data/fonts/MonaspaceRadon/MonaspaceRadon-Italic.otf
+-rw-r--r--   0        0        0    88668 2024-04-08 04:19:15.429912 pygpt_net-2.2.2/src/pygpt_net/data/fonts/MonaspaceRadon/MonaspaceRadon-Regular.otf
+-rw-r--r--   0        0        0    79280 2024-04-08 04:19:15.429912 pygpt_net-2.2.2/src/pygpt_net/data/fonts/MonaspaceXenon/MonaspaceXenon-Bold.otf
+-rw-r--r--   0        0        0    85648 2024-04-08 04:19:15.429912 pygpt_net-2.2.2/src/pygpt_net/data/fonts/MonaspaceXenon/MonaspaceXenon-BoldItalic.otf
+-rw-r--r--   0        0        0    85824 2024-04-08 04:19:15.429912 pygpt_net-2.2.2/src/pygpt_net/data/fonts/MonaspaceXenon/MonaspaceXenon-Italic.otf
+-rw-r--r--   0        0        0    80200 2024-04-08 04:19:15.429912 pygpt_net-2.2.2/src/pygpt_net/data/fonts/MonaspaceXenon/MonaspaceXenon-Regular.otf
+-rwxr-xr-x   0        0        0     4352 2024-03-18 04:54:07.633826 pygpt_net-2.2.2/src/pygpt_net/data/fonts/SpaceMono/OFL.txt
+-rwxr-xr-x   0        0        0    86636 2024-03-18 04:54:07.633826 pygpt_net-2.2.2/src/pygpt_net/data/fonts/SpaceMono/SpaceMono-Bold.ttf
+-rwxr-xr-x   0        0        0    95292 2024-03-18 04:54:07.633826 pygpt_net-2.2.2/src/pygpt_net/data/fonts/SpaceMono/SpaceMono-BoldItalic.ttf
+-rwxr-xr-x   0        0        0   103524 2024-03-18 04:54:07.633826 pygpt_net-2.2.2/src/pygpt_net/data/fonts/SpaceMono/SpaceMono-Italic.ttf
+-rwxr-xr-x   0        0        0    90904 2024-03-18 04:54:07.637826 pygpt_net-2.2.2/src/pygpt_net/data/fonts/SpaceMono/SpaceMono-Regular.ttf
+-rwxr-xr-x   0        0        0     3461 2023-04-14 00:10:28.000000 pygpt_net-2.2.2/src/pygpt_net/data/icon.ico
+-rwxr-xr-x   0        0        0    13970 2023-04-14 00:10:28.000000 pygpt_net-2.2.2/src/pygpt_net/data/icon.png
+-rw-r--r--   0        0        0     5471 2024-01-29 18:11:38.035830 pygpt_net-2.2.2/src/pygpt_net/data/icon_tray_busy.ico
+-rw-r--r--   0        0        0    14837 2024-01-29 18:11:38.035830 pygpt_net-2.2.2/src/pygpt_net/data/icon_tray_error.ico
+-rw-r--r--   0        0        0     4209 2024-01-29 18:11:38.035830 pygpt_net-2.2.2/src/pygpt_net/data/icon_tray_idle.ico
+-rw-r--r--   0        0        0      538 2024-01-30 17:23:19.885579 pygpt_net-2.2.2/src/pygpt_net/data/icons/abc.svg
+-rw-r--r--   0        0        0      178 2024-01-30 17:23:19.885579 pygpt_net-2.2.2/src/pygpt_net/data/icons/add.svg
+-rw-r--r--   0        0        0      463 2024-01-30 17:23:19.885579 pygpt_net-2.2.2/src/pygpt_net/data/icons/add_circle.svg
+-rw-r--r--   0        0        0      348 2024-01-30 17:23:19.885579 pygpt_net-2.2.2/src/pygpt_net/data/icons/add_folder.svg
+-rw-r--r--   0        0        0      391 2024-01-30 17:23:19.885579 pygpt_net-2.2.2/src/pygpt_net/data/icons/add_library.svg
+-rw-r--r--   0        0        0      558 2024-01-30 17:23:19.885579 pygpt_net-2.2.2/src/pygpt_net/data/icons/alarm.svg
+-rw-r--r--   0        0        0     1027 2024-01-30 17:23:19.885579 pygpt_net-2.2.2/src/pygpt_net/data/icons/apps.svg
+-rw-r--r--   0        0        0      267 2024-01-30 17:23:19.885579 pygpt_net-2.2.2/src/pygpt_net/data/icons/asterisk.svg
+-rw-r--r--   0        0        0      429 2024-01-30 17:23:19.885579 pygpt_net-2.2.2/src/pygpt_net/data/icons/attachment.svg
+-rw-r--r--   0        0        0      422 2024-01-30 17:23:19.885579 pygpt_net-2.2.2/src/pygpt_net/data/icons/attachments.svg
+-rw-r--r--   0        0        0      185 2024-01-30 17:23:19.885579 pygpt_net-2.2.2/src/pygpt_net/data/icons/back.svg
+-rw-r--r--   0        0        0      395 2024-01-30 17:23:19.885579 pygpt_net-2.2.2/src/pygpt_net/data/icons/backspace.svg
+-rw-r--r--   0        0        0      472 2024-01-30 17:23:19.885579 pygpt_net-2.2.2/src/pygpt_net/data/icons/block.svg
+-rw-r--r--   0        0        0      255 2024-01-30 17:23:19.885579 pygpt_net-2.2.2/src/pygpt_net/data/icons/bookmark.svg
+-rw-r--r--   0        0        0      423 2024-01-30 17:23:19.885579 pygpt_net-2.2.2/src/pygpt_net/data/icons/brush.svg
+-rw-r--r--   0        0        0      523 2024-01-30 17:23:19.885579 pygpt_net-2.2.2/src/pygpt_net/data/icons/build.svg
+-rw-r--r--   0        0        0      927 2024-01-30 17:23:19.885579 pygpt_net-2.2.2/src/pygpt_net/data/icons/calendar.svg
+-rw-r--r--   0        0        0      496 2024-01-30 17:23:19.885579 pygpt_net-2.2.2/src/pygpt_net/data/icons/camera.svg
+-rw-r--r--   0        0        0      987 2024-03-09 21:41:28.185853 pygpt_net-2.2.2/src/pygpt_net/data/icons/chat/audio.png
+-rw-r--r--   0        0        0      798 2024-03-09 21:41:28.185853 pygpt_net-2.2.2/src/pygpt_net/data/icons/chat/copy.png
+-rw-r--r--   0        0        0      737 2024-03-09 21:41:28.185853 pygpt_net-2.2.2/src/pygpt_net/data/icons/chat/delete.png
+-rw-r--r--   0        0        0      837 2024-03-09 21:41:28.185853 pygpt_net-2.2.2/src/pygpt_net/data/icons/chat/edit.png
+-rw-r--r--   0        0        0      715 2024-03-10 08:19:22.357281 pygpt_net-2.2.2/src/pygpt_net/data/icons/chat/join.png
+-rw-r--r--   0        0        0      956 2024-03-09 21:41:28.185853 pygpt_net-2.2.2/src/pygpt_net/data/icons/chat/reload.png
+-rw-r--r--   0        0        0      336 2024-01-30 17:23:19.885579 pygpt_net-2.2.2/src/pygpt_net/data/icons/chat.svg
+-rw-r--r--   0        0        0      174 2024-01-30 17:23:19.885579 pygpt_net-2.2.2/src/pygpt_net/data/icons/check.svg
+-rw-r--r--   0        0        0      459 2024-01-30 17:23:19.885579 pygpt_net-2.2.2/src/pygpt_net/data/icons/check_circle.svg
+-rw-r--r--   0        0        0      265 2024-01-30 17:23:19.885579 pygpt_net-2.2.2/src/pygpt_net/data/icons/checklist.svg
+-rw-r--r--   0        0        0      406 2024-01-30 17:23:19.885579 pygpt_net-2.2.2/src/pygpt_net/data/icons/circle.svg
+-rw-r--r--   0        0        0      191 2024-01-30 17:23:19.885579 pygpt_net-2.2.2/src/pygpt_net/data/icons/clear.svg
+-rw-r--r--   0        0        0      411 2024-01-30 17:23:19.885579 pygpt_net-2.2.2/src/pygpt_net/data/icons/clock.svg
+-rw-r--r--   0        0        0      218 2024-01-30 17:23:19.885579 pygpt_net-2.2.2/src/pygpt_net/data/icons/close.svg
+-rw-r--r--   0        0        0      503 2024-01-30 17:23:19.885579 pygpt_net-2.2.2/src/pygpt_net/data/icons/close_circle.svg
+-rw-r--r--   0        0        0      224 2024-01-30 17:23:19.885579 pygpt_net-2.2.2/src/pygpt_net/data/icons/code.svg
+-rw-r--r--   0        0        0      298 2024-01-30 17:23:19.885579 pygpt_net-2.2.2/src/pygpt_net/data/icons/computer.svg
+-rw-r--r--   0        0        0      336 2024-01-30 17:23:19.885579 pygpt_net-2.2.2/src/pygpt_net/data/icons/copy.svg
+-rw-r--r--   0        0        0      264 2024-01-30 17:23:19.885579 pygpt_net-2.2.2/src/pygpt_net/data/icons/crop.svg
+-rw-r--r--   0        0        0      666 2024-01-30 17:23:19.885579 pygpt_net-2.2.2/src/pygpt_net/data/icons/cut.svg
+-rw-r--r--   0        0        0      725 2024-01-30 17:23:19.885579 pygpt_net-2.2.2/src/pygpt_net/data/icons/db.svg
+-rw-r--r--   0        0        0      271 2024-01-30 17:23:19.889579 pygpt_net-2.2.2/src/pygpt_net/data/icons/delete.svg
+-rw-r--r--   0        0        0      174 2024-01-30 17:23:19.889579 pygpt_net-2.2.2/src/pygpt_net/data/icons/done.svg
+-rw-r--r--   0        0        0      274 2024-01-30 17:23:19.889579 pygpt_net-2.2.2/src/pygpt_net/data/icons/download.svg
+-rw-r--r--   0        0        0      283 2024-01-30 17:23:19.889579 pygpt_net-2.2.2/src/pygpt_net/data/icons/draft.svg
+-rw-r--r--   0        0        0      323 2024-01-30 17:23:19.889579 pygpt_net-2.2.2/src/pygpt_net/data/icons/drag.svg
+-rw-r--r--   0        0        0      325 2024-01-30 17:23:19.889579 pygpt_net-2.2.2/src/pygpt_net/data/icons/edit.svg
+-rw-r--r--   0        0        0      497 2024-01-30 17:23:19.889579 pygpt_net-2.2.2/src/pygpt_net/data/icons/emergency.svg
+-rw-r--r--   0        0        0      195 2024-01-30 17:23:19.889579 pygpt_net-2.2.2/src/pygpt_net/data/icons/equalizer.svg
+-rw-r--r--   0        0        0      533 2024-01-30 17:23:19.889579 pygpt_net-2.2.2/src/pygpt_net/data/icons/error.svg
+-rw-r--r--   0        0        0      372 2024-01-30 17:23:19.889579 pygpt_net-2.2.2/src/pygpt_net/data/icons/event_available.svg
+-rw-r--r--   0        0        0      174 2024-01-30 17:23:19.889579 pygpt_net-2.2.2/src/pygpt_net/data/icons/expand.svg
+-rw-r--r--   0        0        0      247 2024-01-30 17:23:19.889579 pygpt_net-2.2.2/src/pygpt_net/data/icons/fast_forward.svg
+-rw-r--r--   0        0        0      250 2024-01-30 17:23:19.889579 pygpt_net-2.2.2/src/pygpt_net/data/icons/fast_rewind.svg
+-rw-r--r--   0        0        0      504 2024-01-30 17:23:19.889579 pygpt_net-2.2.2/src/pygpt_net/data/icons/favorite.svg
+-rw-r--r--   0        0        0      297 2024-01-30 17:23:19.889579 pygpt_net-2.2.2/src/pygpt_net/data/icons/folder.svg
+-rw-r--r--   0        0        0      249 2024-01-30 17:23:19.889579 pygpt_net-2.2.2/src/pygpt_net/data/icons/folder_filled.svg
+-rw-r--r--   0        0        0      186 2024-01-30 17:23:19.889579 pygpt_net-2.2.2/src/pygpt_net/data/icons/forward.svg
+-rw-r--r--   0        0        0      194 2024-01-30 17:23:19.889579 pygpt_net-2.2.2/src/pygpt_net/data/icons/full.svg
+-rw-r--r--   0        0        0      249 2024-01-30 17:23:19.889579 pygpt_net-2.2.2/src/pygpt_net/data/icons/fullscreen.svg
+-rw-r--r--   0        0        0      459 2024-01-30 17:23:19.889579 pygpt_net-2.2.2/src/pygpt_net/data/icons/grid.svg
+-rw-r--r--   0        0        0      602 2024-01-30 17:23:19.889579 pygpt_net-2.2.2/src/pygpt_net/data/icons/hearing.svg
+-rw-r--r--   0        0        0      691 2024-01-30 17:23:19.889579 pygpt_net-2.2.2/src/pygpt_net/data/icons/help.svg
+-rw-r--r--   0        0        0      440 2024-01-30 17:23:19.889579 pygpt_net-2.2.2/src/pygpt_net/data/icons/history.svg
+-rw-r--r--   0        0        0      239 2024-01-30 17:23:19.889579 pygpt_net-2.2.2/src/pygpt_net/data/icons/home.svg
+-rw-r--r--   0        0        0      176 2024-01-30 17:23:19.889579 pygpt_net-2.2.2/src/pygpt_net/data/icons/home_filled.svg
+-rw-r--r--   0        0        0      323 2024-01-30 17:23:19.889579 pygpt_net-2.2.2/src/pygpt_net/data/icons/image.svg
+-rw-r--r--   0        0        0      531 2024-01-30 17:23:19.889579 pygpt_net-2.2.2/src/pygpt_net/data/icons/info.svg
+-rw-r--r--   0        0        0      337 2024-01-30 17:23:19.889579 pygpt_net-2.2.2/src/pygpt_net/data/icons/input.svg
+-rw-r--r--   0        0        0      541 2024-01-30 17:23:19.889579 pygpt_net-2.2.2/src/pygpt_net/data/icons/key.svg
+-rw-r--r--   0        0        0      517 2024-01-30 17:23:19.889579 pygpt_net-2.2.2/src/pygpt_net/data/icons/keyboard.svg
+-rw-r--r--   0        0        0      972 2024-01-30 17:23:19.889579 pygpt_net-2.2.2/src/pygpt_net/data/icons/language.svg
+-rw-r--r--   0        0        0      491 2024-01-30 17:23:19.889579 pygpt_net-2.2.2/src/pygpt_net/data/icons/list.svg
+-rw-r--r--   0        0        0      495 2024-01-30 17:23:19.889579 pygpt_net-2.2.2/src/pygpt_net/data/icons/lock.svg
+-rw-r--r--   0        0        0      273 2024-01-30 17:23:19.889579 pygpt_net-2.2.2/src/pygpt_net/data/icons/logout.svg
+-rw-r--r--   0        0        0      392 2024-01-30 17:23:19.889579 pygpt_net-2.2.2/src/pygpt_net/data/icons/map.svg
+-rw-r--r--   0        0        0      431 2024-01-30 17:23:19.889579 pygpt_net-2.2.2/src/pygpt_net/data/icons/memory.svg
+-rw-r--r--   0        0        0      189 2024-01-30 17:23:19.889579 pygpt_net-2.2.2/src/pygpt_net/data/icons/menu.svg
+-rw-r--r--   0        0        0      447 2024-01-30 17:23:19.889579 pygpt_net-2.2.2/src/pygpt_net/data/icons/mic.svg
+-rw-r--r--   0        0        0      485 2024-01-30 17:23:19.889579 pygpt_net-2.2.2/src/pygpt_net/data/icons/mic_off.svg
+-rw-r--r--   0        0        0      423 2024-01-30 17:23:19.889579 pygpt_net-2.2.2/src/pygpt_net/data/icons/more_horizontal.svg
+-rw-r--r--   0        0        0      491 2024-01-30 17:23:19.889579 pygpt_net-2.2.2/src/pygpt_net/data/icons/mute.svg
+-rw-r--r--   0        0        0      296 2024-01-30 17:23:19.889579 pygpt_net-2.2.2/src/pygpt_net/data/icons/open_tab.svg
+-rw-r--r--   0        0        0      846 2024-01-30 17:23:19.889579 pygpt_net-2.2.2/src/pygpt_net/data/icons/palette.svg
+-rw-r--r--   0        0        0      431 2024-01-30 17:23:19.889579 pygpt_net-2.2.2/src/pygpt_net/data/icons/paste.svg
+-rw-r--r--   0        0        0      250 2024-01-30 17:23:19.889579 pygpt_net-2.2.2/src/pygpt_net/data/icons/pause.svg
+-rw-r--r--   0        0        0      454 2024-01-30 17:23:19.889579 pygpt_net-2.2.2/src/pygpt_net/data/icons/pause_circle.svg
+-rw-r--r--   0        0        0      377 2024-01-30 17:23:19.889579 pygpt_net-2.2.2/src/pygpt_net/data/icons/photos.svg
+-rw-r--r--   0        0        0      441 2024-01-30 17:23:19.889579 pygpt_net-2.2.2/src/pygpt_net/data/icons/pin.svg
+-rw-r--r--   0        0        0      186 2024-01-30 17:23:19.889579 pygpt_net-2.2.2/src/pygpt_net/data/icons/play.svg
+-rw-r--r--   0        0        0      197 2024-01-30 17:23:19.889579 pygpt_net-2.2.2/src/pygpt_net/data/icons/play_pause.svg
+-rw-r--r--   0        0        0      246 2024-01-30 17:23:19.889579 pygpt_net-2.2.2/src/pygpt_net/data/icons/playlist_add.svg
+-rw-r--r--   0        0        0      318 2024-01-30 17:23:19.889579 pygpt_net-2.2.2/src/pygpt_net/data/icons/power.svg
+-rw-r--r--   0        0        0      478 2024-01-30 17:23:19.889579 pygpt_net-2.2.2/src/pygpt_net/data/icons/print.svg
+-rw-r--r--   0        0        0      598 2024-01-30 17:23:19.889579 pygpt_net-2.2.2/src/pygpt_net/data/icons/public_filled.svg
+-rw-r--r--   0        0        0      283 2024-01-30 20:56:32.772879 pygpt_net-2.2.2/src/pygpt_net/data/icons/redo.svg
+-rw-r--r--   0        0        0      329 2024-01-30 17:23:19.889579 pygpt_net-2.2.2/src/pygpt_net/data/icons/reload.svg
+-rw-r--r--   0        0        0      260 2024-01-30 17:23:19.889579 pygpt_net-2.2.2/src/pygpt_net/data/icons/repeat.svg
+-rw-r--r--   0        0        0      400 2024-01-30 17:23:19.889579 pygpt_net-2.2.2/src/pygpt_net/data/icons/replay.svg
+-rw-r--r--   0        0        0      401 2024-01-30 17:23:19.889579 pygpt_net-2.2.2/src/pygpt_net/data/icons/resize.svg
+-rw-r--r--   0        0        0      615 2024-01-30 17:23:19.889579 pygpt_net-2.2.2/src/pygpt_net/data/icons/robot.svg
+-rw-r--r--   0        0        0      807 2024-01-30 17:23:19.889579 pygpt_net-2.2.2/src/pygpt_net/data/icons/router.svg
+-rw-r--r--   0        0        0      384 2024-01-30 17:23:19.889579 pygpt_net-2.2.2/src/pygpt_net/data/icons/save.svg
+-rw-r--r--   0        0        0      469 2024-01-30 17:23:19.889579 pygpt_net-2.2.2/src/pygpt_net/data/icons/schedule.svg
+-rw-r--r--   0        0        0      396 2024-01-30 17:23:19.889579 pygpt_net-2.2.2/src/pygpt_net/data/icons/screenshot.svg
+-rw-r--r--   0        0        0      372 2024-01-30 17:23:19.889579 pygpt_net-2.2.2/src/pygpt_net/data/icons/search.svg
+-rw-r--r--   0        0        0      274 2024-01-30 17:23:19.889579 pygpt_net-2.2.2/src/pygpt_net/data/icons/security.svg
+-rw-r--r--   0        0        0      660 2024-01-30 17:23:19.889579 pygpt_net-2.2.2/src/pygpt_net/data/icons/sensors.svg
+-rw-r--r--   0        0        0      767 2024-01-30 17:23:19.889579 pygpt_net-2.2.2/src/pygpt_net/data/icons/settings.svg
+-rw-r--r--   0        0        0      475 2024-01-30 17:23:19.889579 pygpt_net-2.2.2/src/pygpt_net/data/icons/settings_filled.svg
+-rw-r--r--   0        0        0      792 2024-01-30 17:23:19.889579 pygpt_net-2.2.2/src/pygpt_net/data/icons/share.svg
+-rw-r--r--   0        0        0      469 2024-01-30 17:23:19.889579 pygpt_net-2.2.2/src/pygpt_net/data/icons/shedule.svg
+-rw-r--r--   0        0        0      189 2024-01-30 17:23:19.889579 pygpt_net-2.2.2/src/pygpt_net/data/icons/sort.svg
+-rw-r--r--   0        0        0      386 2024-01-30 17:23:19.889579 pygpt_net-2.2.2/src/pygpt_net/data/icons/stack.svg
+-rw-r--r--   0        0        0      306 2024-01-30 17:23:19.889579 pygpt_net-2.2.2/src/pygpt_net/data/icons/stacks.svg
+-rw-r--r--   0        0        0      291 2024-01-30 17:23:19.889579 pygpt_net-2.2.2/src/pygpt_net/data/icons/star.svg
+-rw-r--r--   0        0        0      188 2024-01-30 17:23:19.893578 pygpt_net-2.2.2/src/pygpt_net/data/icons/stop.svg
+-rw-r--r--   0        0        0      432 2024-01-30 17:23:19.893578 pygpt_net-2.2.2/src/pygpt_net/data/icons/stop_circle.svg
+-rw-r--r--   0        0        0      381 2024-01-30 17:23:19.893578 pygpt_net-2.2.2/src/pygpt_net/data/icons/sync.svg
+-rw-r--r--   0        0        0      317 2024-01-30 17:23:19.893578 pygpt_net-2.2.2/src/pygpt_net/data/icons/tag.svg
+-rw-r--r--   0        0        0      334 2024-01-30 17:23:19.893578 pygpt_net-2.2.2/src/pygpt_net/data/icons/task.svg
+-rw-r--r--   0        0        0      336 2024-01-30 17:23:19.893578 pygpt_net-2.2.2/src/pygpt_net/data/icons/terminal.svg
+-rw-r--r--   0        0        0      204 2024-01-30 17:23:19.893578 pygpt_net-2.2.2/src/pygpt_net/data/icons/text.svg
+-rw-r--r--   0        0        0      329 2024-01-30 17:23:19.893578 pygpt_net-2.2.2/src/pygpt_net/data/icons/textfile.svg
+-rw-r--r--   0        0        0      479 2024-01-30 17:23:19.893578 pygpt_net-2.2.2/src/pygpt_net/data/icons/timer.svg
+-rw-r--r--   0        0        0      321 2024-01-30 17:23:19.893578 pygpt_net-2.2.2/src/pygpt_net/data/icons/today.svg
+-rw-r--r--   0        0        0      308 2024-01-30 17:23:19.893578 pygpt_net-2.2.2/src/pygpt_net/data/icons/tune.svg
+-rw-r--r--   0        0        0      282 2024-01-30 17:23:19.893578 pygpt_net-2.2.2/src/pygpt_net/data/icons/undo.svg
+-rw-r--r--   0        0        0      444 2024-01-30 17:23:19.893578 pygpt_net-2.2.2/src/pygpt_net/data/icons/update.svg
+-rw-r--r--   0        0        0      392 2024-01-30 17:23:19.893578 pygpt_net-2.2.2/src/pygpt_net/data/icons/updater.svg
+-rw-r--r--   0        0        0      276 2024-01-30 17:23:19.893578 pygpt_net-2.2.2/src/pygpt_net/data/icons/upload.svg
+-rw-r--r--   0        0        0      339 2024-01-30 17:23:19.893578 pygpt_net-2.2.2/src/pygpt_net/data/icons/video.svg
+-rw-r--r--   0        0        0      550 2024-01-30 17:23:19.893578 pygpt_net-2.2.2/src/pygpt_net/data/icons/view.svg
+-rw-r--r--   0        0        0      736 2024-01-30 17:23:19.893578 pygpt_net-2.2.2/src/pygpt_net/data/icons/voice.svg
+-rw-r--r--   0        0        0      374 2024-01-30 17:23:19.893578 pygpt_net-2.2.2/src/pygpt_net/data/icons/volume.svg
+-rw-r--r--   0        0        0      310 2024-01-30 17:23:19.893578 pygpt_net-2.2.2/src/pygpt_net/data/icons/warning.svg
+-rw-r--r--   0        0        0      300 2024-01-30 17:23:19.893578 pygpt_net-2.2.2/src/pygpt_net/data/icons/webcam.svg
+-rw-r--r--   0        0        0      375 2024-02-29 03:07:51.274132 pygpt_net-2.2.2/src/pygpt_net/data/icons/webcam_off.svg
+-rw-r--r--   0        0        0      325 2024-01-30 17:23:19.893578 pygpt_net-2.2.2/src/pygpt_net/data/icons/width.svg
+-rw-r--r--   0        0        0      336 2024-01-30 17:23:19.893578 pygpt_net-2.2.2/src/pygpt_net/data/icons/window.svg
+-rw-r--r--   0        0        0      365 2024-01-30 17:23:19.893578 pygpt_net-2.2.2/src/pygpt_net/data/icons/work.svg
+-rw-r--r--   0        0        0      422 2024-01-30 17:23:19.893578 pygpt_net-2.2.2/src/pygpt_net/data/icons/zoom_in.svg
+-rw-r--r--   0        0        0      396 2024-01-30 17:23:19.893578 pygpt_net-2.2.2/src/pygpt_net/data/icons/zoom_out.svg
+-rwxr-xr-x   0        0        0    45202 2024-04-29 05:51:11.640212 pygpt_net-2.2.2/src/pygpt_net/data/locale/locale.de.ini
+-rwxr-xr-x   0        0        0    53570 2024-04-29 05:51:11.640212 pygpt_net-2.2.2/src/pygpt_net/data/locale/locale.en.ini
+-rwxr-xr-x   0        0        0    45375 2024-04-29 05:51:11.640212 pygpt_net-2.2.2/src/pygpt_net/data/locale/locale.es.ini
+-rwxr-xr-x   0        0        0    47002 2024-04-29 05:51:11.644212 pygpt_net-2.2.2/src/pygpt_net/data/locale/locale.fr.ini
+-rwxr-xr-x   0        0        0    44458 2024-04-29 05:51:11.644212 pygpt_net-2.2.2/src/pygpt_net/data/locale/locale.it.ini
+-rwxr-xr-x   0        0        0    44360 2024-04-29 05:51:11.644212 pygpt_net-2.2.2/src/pygpt_net/data/locale/locale.pl.ini
+-rwxr-xr-x   0        0        0    62630 2024-04-29 05:51:11.644212 pygpt_net-2.2.2/src/pygpt_net/data/locale/locale.uk.ini
+-rwxr-xr-x   0        0        0    48131 2024-04-29 05:51:11.644212 pygpt_net-2.2.2/src/pygpt_net/data/locale/locale.zh.ini
+-rwxr-xr-x   0        0        0     1477 2024-03-12 06:49:17.164785 pygpt_net-2.2.2/src/pygpt_net/data/locale/plugin.agent.en.ini
+-rwxr-xr-x   0        0        0     1394 2024-03-12 06:49:17.164785 pygpt_net-2.2.2/src/pygpt_net/data/locale/plugin.agent.pl.ini
+-rwxr-xr-x   0        0        0     5371 2024-03-12 06:49:17.168786 pygpt_net-2.2.2/src/pygpt_net/data/locale/plugin.audio_input.en.ini
+-rwxr-xr-x   0        0        0     5129 2024-03-12 06:49:17.168786 pygpt_net-2.2.2/src/pygpt_net/data/locale/plugin.audio_input.pl.ini
+-rwxr-xr-x   0        0        0     1721 2024-03-12 06:49:17.168786 pygpt_net-2.2.2/src/pygpt_net/data/locale/plugin.audio_output.en.ini
+-rwxr-xr-x   0        0        0     1395 2024-03-12 06:49:17.168786 pygpt_net-2.2.2/src/pygpt_net/data/locale/plugin.audio_output.pl.ini
+-rw-r--r--   0        0        0      622 2024-03-12 06:49:17.168786 pygpt_net-2.2.2/src/pygpt_net/data/locale/plugin.cmd_api.en.ini
+-rw-r--r--   0        0        0      853 2024-03-12 06:49:17.168786 pygpt_net-2.2.2/src/pygpt_net/data/locale/plugin.cmd_api.pl.ini
+-rwxr-xr-x   0        0        0     2365 2024-03-19 03:42:00.618910 pygpt_net-2.2.2/src/pygpt_net/data/locale/plugin.cmd_code_interpreter.en.ini
+-rwxr-xr-x   0        0        0     1614 2024-03-12 06:49:17.168786 pygpt_net-2.2.2/src/pygpt_net/data/locale/plugin.cmd_code_interpreter.pl.ini
+-rwxr-xr-x   0        0        0      455 2024-03-12 06:49:17.168786 pygpt_net-2.2.2/src/pygpt_net/data/locale/plugin.cmd_custom.en.ini
+-rwxr-xr-x   0        0        0      528 2024-03-12 06:49:17.168786 pygpt_net-2.2.2/src/pygpt_net/data/locale/plugin.cmd_custom.pl.ini
+-rwxr-xr-x   0        0        0     4234 2024-03-13 17:35:47.179523 pygpt_net-2.2.2/src/pygpt_net/data/locale/plugin.cmd_files.en.ini
+-rwxr-xr-x   0        0        0     3584 2024-03-13 17:35:47.179523 pygpt_net-2.2.2/src/pygpt_net/data/locale/plugin.cmd_files.pl.ini
+-rw-r--r--   0        0        0     2280 2024-03-12 06:49:17.168786 pygpt_net-2.2.2/src/pygpt_net/data/locale/plugin.cmd_history.en.ini
+-rw-r--r--   0        0        0     2765 2024-03-12 06:49:17.168786 pygpt_net-2.2.2/src/pygpt_net/data/locale/plugin.cmd_history.pl.ini
+-rw-r--r--   0        0        0     1042 2024-03-12 06:49:17.168786 pygpt_net-2.2.2/src/pygpt_net/data/locale/plugin.cmd_serial.en.ini
+-rw-r--r--   0        0        0     1511 2024-03-12 06:49:17.168786 pygpt_net-2.2.2/src/pygpt_net/data/locale/plugin.cmd_serial.pl.ini
+-rwxr-xr-x   0        0        0     4840 2024-03-12 06:49:17.168786 pygpt_net-2.2.2/src/pygpt_net/data/locale/plugin.cmd_web.en.ini
+-rwxr-xr-x   0        0        0     4660 2024-03-12 06:49:17.168786 pygpt_net-2.2.2/src/pygpt_net/data/locale/plugin.cmd_web.pl.ini
+-rw-r--r--   0        0        0      758 2024-03-12 06:49:17.168786 pygpt_net-2.2.2/src/pygpt_net/data/locale/plugin.crontab.en.ini
+-rw-r--r--   0        0        0      871 2024-03-12 06:49:17.168786 pygpt_net-2.2.2/src/pygpt_net/data/locale/plugin.crontab.pl.ini
+-rw-r--r--   0        0        0      338 2024-03-12 06:49:17.168786 pygpt_net-2.2.2/src/pygpt_net/data/locale/plugin.extra_prompt.en.ini
+-rw-r--r--   0        0        0      474 2024-03-12 03:34:38.663323 pygpt_net-2.2.2/src/pygpt_net/data/locale/plugin.extra_prompt.pl.ini
+-rwxr-xr-x   0        0        0     1970 2024-03-13 17:35:47.179523 pygpt_net-2.2.2/src/pygpt_net/data/locale/plugin.idx_llama_index.en.ini
+-rwxr-xr-x   0        0        0     1180 2024-03-13 17:35:47.179523 pygpt_net-2.2.2/src/pygpt_net/data/locale/plugin.idx_llama_index.pl.ini
+-rw-r--r--   0        0        0      396 2024-03-17 13:18:45.662349 pygpt_net-2.2.2/src/pygpt_net/data/locale/plugin.openai_dalle.en.ini
+-rw-r--r--   0        0        0      427 2024-03-17 13:18:45.662349 pygpt_net-2.2.2/src/pygpt_net/data/locale/plugin.openai_dalle.pl.ini
+-rw-r--r--   0        0        0     1393 2024-03-12 06:49:17.168786 pygpt_net-2.2.2/src/pygpt_net/data/locale/plugin.openai_vision.en.ini
+-rw-r--r--   0        0        0     1426 2024-03-12 06:49:17.168786 pygpt_net-2.2.2/src/pygpt_net/data/locale/plugin.openai_vision.pl.ini
+-rwxr-xr-x   0        0        0      631 2024-01-30 20:56:32.776879 pygpt_net-2.2.2/src/pygpt_net/data/locale/plugin.real_time.en.ini
+-rwxr-xr-x   0        0        0      752 2024-01-30 20:56:32.776879 pygpt_net-2.2.2/src/pygpt_net/data/locale/plugin.real_time.pl.ini
+-rwxr-xr-x   0        0        0    19418 2023-12-14 19:08:45.000000 pygpt_net-2.2.2/src/pygpt_net/data/logo.png
+-rw-r--r--   0        0        0    83051 2024-04-22 22:35:26.800429 pygpt_net-2.2.2/src/pygpt_net/data/prompts.csv
+-rwxr-xr-x   0        0        0    31708 2024-02-20 19:10:03.189314 pygpt_net-2.2.2/src/pygpt_net/data/win32/README.rtf
+-rwxr-xr-x   0        0        0     1633 2023-04-14 00:10:28.000000 pygpt_net-2.2.2/src/pygpt_net/data/win32/USER-LICENSE.rtf
+-rwxr-xr-x   0        0        0    87160 2023-04-14 00:10:28.000000 pygpt_net-2.2.2/src/pygpt_net/data/win32/pygpt.aip
+-rwxr-xr-x   0        0        0       45 2023-12-19 15:40:13.000000 pygpt_net-2.2.2/src/pygpt_net/data/win32/qt.conf
+-rw-r--r--   0        0        0    21736 2024-03-02 20:04:01.386329 pygpt_net-2.2.2/src/pygpt_net/icons.qrc
+-rw-r--r--   0        0        0    90430 2024-03-02 20:05:43.048414 pygpt_net-2.2.2/src/pygpt_net/icons_rc.py
+-rw-r--r--   0        0        0      488 2023-12-31 03:12:36.955235 pygpt_net-2.2.2/src/pygpt_net/item/__init__.py
+-rw-r--r--   0        0        0     9587 2024-04-26 21:55:50.679597 pygpt_net-2.2.2/src/pygpt_net/item/assistant.py
+-rw-r--r--   0        0        0     2110 2024-04-26 21:55:50.679597 pygpt_net-2.2.2/src/pygpt_net/item/attachment.py
+-rw-r--r--   0        0        0     2108 2024-01-27 21:42:30.960980 pygpt_net-2.2.2/src/pygpt_net/item/calendar_note.py
+-rw-r--r--   0        0        0    11499 2024-04-29 05:51:11.644212 pygpt_net-2.2.2/src/pygpt_net/item/ctx.py
+-rw-r--r--   0        0        0     1681 2024-01-27 21:42:30.960980 pygpt_net-2.2.2/src/pygpt_net/item/index.py
+-rw-r--r--   0        0        0      600 2023-12-31 03:12:34.283242 pygpt_net-2.2.2/src/pygpt_net/item/mode.py
+-rw-r--r--   0        0        0     6208 2024-01-27 21:42:30.960980 pygpt_net-2.2.2/src/pygpt_net/item/model.py
+-rw-r--r--   0        0        0     1508 2024-01-27 21:42:30.960980 pygpt_net-2.2.2/src/pygpt_net/item/notepad.py
+-rw-r--r--   0        0        0     4052 2024-02-15 05:07:04.122540 pygpt_net-2.2.2/src/pygpt_net/item/preset.py
+-rwxr-xr-x   0        0        0     7995 2024-04-21 18:06:27.128064 pygpt_net-2.2.2/src/pygpt_net/launcher.py
+-rw-r--r--   0        0        0     2849 2023-12-28 02:55:13.572642 pygpt_net-2.2.2/src/pygpt_net/migrations/Version20231227152900.py
+-rw-r--r--   0        0        0      906 2023-12-30 08:47:37.360628 pygpt_net-2.2.2/src/pygpt_net/migrations/Version20231230095000.py
+-rw-r--r--   0        0        0      901 2024-01-01 00:17:57.553256 pygpt_net-2.2.2/src/pygpt_net/migrations/Version20231231230000.py
+-rw-r--r--   0        0        0     1303 2024-01-06 06:27:36.351928 pygpt_net-2.2.2/src/pygpt_net/migrations/Version20240106060000.py
+-rw-r--r--   0        0        0      865 2024-01-07 09:35:02.638810 pygpt_net-2.2.2/src/pygpt_net/migrations/Version20240107060000.py
+-rw-r--r--   0        0        0     1756 2024-02-23 01:50:39.602419 pygpt_net-2.2.2/src/pygpt_net/migrations/Version20240222160000.py
+-rw-r--r--   0        0        0     1099 2024-02-23 06:06:25.510176 pygpt_net-2.2.2/src/pygpt_net/migrations/Version20240223050000.py
+-rw-r--r--   0        0        0      847 2024-03-03 22:43:17.403437 pygpt_net-2.2.2/src/pygpt_net/migrations/Version20240303190000.py
+-rw-r--r--   0        0        0     1110 2024-04-10 01:07:30.188635 pygpt_net-2.2.2/src/pygpt_net/migrations/Version20240408180000.py
+-rw-r--r--   0        0        0     1745 2024-04-26 21:55:50.679597 pygpt_net-2.2.2/src/pygpt_net/migrations/Version20240426050000.py
+-rw-r--r--   0        0        0     1862 2024-04-26 21:55:50.679597 pygpt_net-2.2.2/src/pygpt_net/migrations/__init__.py
+-rw-r--r--   0        0        0      614 2023-12-28 02:55:13.572642 pygpt_net-2.2.2/src/pygpt_net/migrations/base.py
+-rwxr-xr-x   0        0        0      488 2023-12-25 22:13:46.802302 pygpt_net-2.2.2/src/pygpt_net/plugin/__init__.py
+-rwxr-xr-x   0        0        0    15161 2024-03-07 01:04:26.445956 pygpt_net-2.2.2/src/pygpt_net/plugin/agent/__init__.py
+-rwxr-xr-x   0        0        0    23567 2024-03-26 17:12:51.294309 pygpt_net-2.2.2/src/pygpt_net/plugin/audio_input/__init__.py
+-rw-r--r--   0        0        0     4669 2024-04-24 23:37:32.612565 pygpt_net-2.2.2/src/pygpt_net/plugin/audio_input/simple.py
+-rwxr-xr-x   0        0        0    10466 2024-03-19 09:04:41.054930 pygpt_net-2.2.2/src/pygpt_net/plugin/audio_input/worker.py
+-rwxr-xr-x   0        0        0     6940 2024-03-10 10:31:05.897000 pygpt_net-2.2.2/src/pygpt_net/plugin/audio_output/__init__.py
+-rw-r--r--   0        0        0     1806 2024-03-10 10:31:05.897000 pygpt_net-2.2.2/src/pygpt_net/plugin/audio_output/worker.py
+-rwxr-xr-x   0        0        0    12704 2024-03-18 04:54:07.637826 pygpt_net-2.2.2/src/pygpt_net/plugin/base.py
+-rwxr-xr-x   0        0        0    11734 2024-03-12 06:49:17.168786 pygpt_net-2.2.2/src/pygpt_net/plugin/cmd_api/__init__.py
+-rw-r--r--   0        0        0     6243 2024-03-16 12:28:31.211383 pygpt_net-2.2.2/src/pygpt_net/plugin/cmd_api/worker.py
+-rwxr-xr-x   0        0        0     9571 2024-03-26 17:12:51.294309 pygpt_net-2.2.2/src/pygpt_net/plugin/cmd_code_interpreter/__init__.py
+-rw-r--r--   0        0        0    14580 2024-04-28 01:03:40.864507 pygpt_net-2.2.2/src/pygpt_net/plugin/cmd_code_interpreter/runner.py
+-rw-r--r--   0        0        0     8841 2024-04-28 01:03:50.072481 pygpt_net-2.2.2/src/pygpt_net/plugin/cmd_code_interpreter/worker.py
+-rwxr-xr-x   0        0        0     5875 2024-03-12 06:49:17.168786 pygpt_net-2.2.2/src/pygpt_net/plugin/cmd_custom/__init__.py
+-rw-r--r--   0        0        0     4507 2024-03-16 12:28:31.211383 pygpt_net-2.2.2/src/pygpt_net/plugin/cmd_custom/worker.py
+-rwxr-xr-x   0        0        0    17031 2024-04-25 01:16:54.112014 pygpt_net-2.2.2/src/pygpt_net/plugin/cmd_files/__init__.py
+-rwxr-xr-x   0        0        0    37969 2024-04-25 01:16:54.112014 pygpt_net-2.2.2/src/pygpt_net/plugin/cmd_files/worker.py
+-rwxr-xr-x   0        0        0    20140 2024-03-16 12:28:31.211383 pygpt_net-2.2.2/src/pygpt_net/plugin/cmd_history/__init__.py
+-rw-r--r--   0        0        0     6673 2024-03-16 12:28:31.211383 pygpt_net-2.2.2/src/pygpt_net/plugin/cmd_history/worker.py
+-rwxr-xr-x   0        0        0     6124 2024-03-16 12:28:31.211383 pygpt_net-2.2.2/src/pygpt_net/plugin/cmd_serial/__init__.py
+-rw-r--r--   0        0        0     8562 2024-03-16 12:28:31.211383 pygpt_net-2.2.2/src/pygpt_net/plugin/cmd_serial/worker.py
+-rwxr-xr-x   0        0        0    21060 2024-03-17 14:26:02.923314 pygpt_net-2.2.2/src/pygpt_net/plugin/cmd_web/__init__.py
+-rwxr-xr-x   0        0        0    12576 2024-02-24 01:55:58.445111 pygpt_net-2.2.2/src/pygpt_net/plugin/cmd_web/websearch.py
+-rw-r--r--   0        0        0    10794 2024-03-26 17:12:51.294309 pygpt_net-2.2.2/src/pygpt_net/plugin/cmd_web/worker.py
+-rwxr-xr-x   0        0        0     8163 2024-03-15 15:31:21.786121 pygpt_net-2.2.2/src/pygpt_net/plugin/crontab/__init__.py
+-rwxr-xr-x   0        0        0     2831 2024-02-18 01:14:49.758062 pygpt_net-2.2.2/src/pygpt_net/plugin/extra_prompt/__init__.py
+-rwxr-xr-x   0        0        0    14334 2024-04-17 01:35:30.426055 pygpt_net-2.2.2/src/pygpt_net/plugin/idx_llama_index/__init__.py
+-rw-r--r--   0        0        0     2825 2024-03-16 16:19:22.432875 pygpt_net-2.2.2/src/pygpt_net/plugin/idx_llama_index/worker.py
+-rwxr-xr-x   0        0        0     6272 2024-03-17 13:18:45.662349 pygpt_net-2.2.2/src/pygpt_net/plugin/openai_dalle/__init__.py
+-rwxr-xr-x   0        0        0    11659 2024-04-11 20:50:24.193030 pygpt_net-2.2.2/src/pygpt_net/plugin/openai_vision/__init__.py
+-rwxr-xr-x   0        0        0     3865 2024-03-17 13:18:45.662349 pygpt_net-2.2.2/src/pygpt_net/plugin/real_time/__init__.py
+-rw-r--r--   0        0        0      488 2023-12-25 22:13:46.802302 pygpt_net-2.2.2/src/pygpt_net/provider/__init__.py
+-rw-r--r--   0        0        0      488 2024-02-24 01:55:58.445111 pygpt_net-2.2.2/src/pygpt_net/provider/audio_input/__init__.py
+-rw-r--r--   0        0        0     1819 2024-02-27 05:21:39.771084 pygpt_net-2.2.2/src/pygpt_net/provider/audio_input/base.py
+-rw-r--r--   0        0        0     2818 2024-02-27 05:21:39.771084 pygpt_net-2.2.2/src/pygpt_net/provider/audio_input/bing_speech_recognition.py
+-rw-r--r--   0        0        0     2904 2024-02-27 05:21:39.771084 pygpt_net-2.2.2/src/pygpt_net/provider/audio_input/google_cloud_speech_recognition.py
+-rw-r--r--   0        0        0     2840 2024-02-27 05:21:39.771084 pygpt_net-2.2.2/src/pygpt_net/provider/audio_input/google_speech_recognition.py
+-rw-r--r--   0        0        0     2244 2024-03-01 03:17:53.457929 pygpt_net-2.2.2/src/pygpt_net/provider/audio_input/openai_whisper.py
+-rw-r--r--   0        0        0     3129 2024-03-01 03:17:53.457929 pygpt_net-2.2.2/src/pygpt_net/provider/audio_input/openai_whisper_local.py
+-rw-r--r--   0        0        0      488 2024-02-24 01:55:58.449111 pygpt_net-2.2.2/src/pygpt_net/provider/audio_output/__init__.py
+-rw-r--r--   0        0        0     1995 2024-02-27 05:21:39.771084 pygpt_net-2.2.2/src/pygpt_net/provider/audio_output/base.py
+-rw-r--r--   0        0        0     4231 2024-02-25 00:27:02.862945 pygpt_net-2.2.2/src/pygpt_net/provider/audio_output/eleven_labs.py
+-rw-r--r--   0        0        0     4286 2024-02-25 00:27:02.862945 pygpt_net-2.2.2/src/pygpt_net/provider/audio_output/google_tts.py
+-rw-r--r--   0        0        0     4960 2024-02-24 01:55:58.449111 pygpt_net-2.2.2/src/pygpt_net/provider/audio_output/ms_azure_tts.py
+-rw-r--r--   0        0        0     3056 2024-02-24 01:55:58.449111 pygpt_net-2.2.2/src/pygpt_net/provider/audio_output/openai_tts.py
+-rw-r--r--   0        0        0      488 2024-01-23 23:46:30.499197 pygpt_net-2.2.2/src/pygpt_net/provider/core/__init__.py
+-rw-r--r--   0        0        0      488 2024-01-23 23:46:30.499197 pygpt_net-2.2.2/src/pygpt_net/provider/core/assistant/__init__.py
+-rw-r--r--   0        0        0     1186 2024-01-23 23:46:30.499197 pygpt_net-2.2.2/src/pygpt_net/provider/core/assistant/base.py
+-rw-r--r--   0        0        0     6399 2024-04-26 21:55:50.679597 pygpt_net-2.2.2/src/pygpt_net/provider/core/assistant/json_file.py
+-rw-r--r--   0        0        0      488 2024-04-26 21:55:50.679597 pygpt_net-2.2.2/src/pygpt_net/provider/core/assistant_file/__init__.py
+-rw-r--r--   0        0        0     1291 2024-04-26 21:55:50.679597 pygpt_net-2.2.2/src/pygpt_net/provider/core/assistant_file/base.py
+-rw-r--r--   0        0        0     5125 2024-04-26 21:55:50.679597 pygpt_net-2.2.2/src/pygpt_net/provider/core/assistant_file/db_sqlite/__init__.py
+-rw-r--r--   0        0        0      885 2024-04-26 21:55:50.679597 pygpt_net-2.2.2/src/pygpt_net/provider/core/assistant_file/db_sqlite/patch.py
+-rw-r--r--   0        0        0    10392 2024-04-26 21:55:50.679597 pygpt_net-2.2.2/src/pygpt_net/provider/core/assistant_file/db_sqlite/storage.py
+-rw-r--r--   0        0        0     1796 2024-04-26 21:55:50.679597 pygpt_net-2.2.2/src/pygpt_net/provider/core/assistant_file/db_sqlite/utils.py
+-rw-r--r--   0        0        0      488 2024-04-26 21:55:50.679597 pygpt_net-2.2.2/src/pygpt_net/provider/core/assistant_store/__init__.py
+-rw-r--r--   0        0        0     1314 2024-04-26 21:55:50.679597 pygpt_net-2.2.2/src/pygpt_net/provider/core/assistant_store/base.py
+-rw-r--r--   0        0        0     3557 2024-04-26 21:55:50.679597 pygpt_net-2.2.2/src/pygpt_net/provider/core/assistant_store/db_sqlite/__init__.py
+-rw-r--r--   0        0        0      885 2024-04-26 21:55:50.679597 pygpt_net-2.2.2/src/pygpt_net/provider/core/assistant_store/db_sqlite/patch.py
+-rw-r--r--   0        0        0     7438 2024-04-26 21:55:50.679597 pygpt_net-2.2.2/src/pygpt_net/provider/core/assistant_store/db_sqlite/storage.py
+-rw-r--r--   0        0        0     2120 2024-04-26 21:55:50.679597 pygpt_net-2.2.2/src/pygpt_net/provider/core/assistant_store/db_sqlite/utils.py
+-rw-r--r--   0        0        0     4377 2024-04-26 21:55:50.679597 pygpt_net-2.2.2/src/pygpt_net/provider/core/assistant_store/json_file.py
+-rw-r--r--   0        0        0      488 2024-01-23 23:46:30.499197 pygpt_net-2.2.2/src/pygpt_net/provider/core/attachment/__init__.py
+-rw-r--r--   0        0        0     1204 2024-01-23 23:46:30.499197 pygpt_net-2.2.2/src/pygpt_net/provider/core/attachment/base.py
+-rw-r--r--   0        0        0     5404 2024-04-26 21:55:50.679597 pygpt_net-2.2.2/src/pygpt_net/provider/core/attachment/json_file.py
+-rw-r--r--   0        0        0      488 2024-01-23 23:46:30.499197 pygpt_net-2.2.2/src/pygpt_net/provider/core/calendar/__init__.py
+-rw-r--r--   0        0        0     1322 2024-01-23 23:46:30.499197 pygpt_net-2.2.2/src/pygpt_net/provider/core/calendar/base.py
+-rw-r--r--   0        0        0     3953 2024-03-08 00:36:17.343108 pygpt_net-2.2.2/src/pygpt_net/provider/core/calendar/db_sqlite/__init__.py
+-rw-r--r--   0        0        0      837 2024-01-23 23:46:30.499197 pygpt_net-2.2.2/src/pygpt_net/provider/core/calendar/db_sqlite/patch.py
+-rw-r--r--   0        0        0    11113 2024-03-07 01:04:26.445956 pygpt_net-2.2.2/src/pygpt_net/provider/core/calendar/db_sqlite/storage.py
+-rw-r--r--   0        0        0      488 2024-01-23 23:46:30.499197 pygpt_net-2.2.2/src/pygpt_net/provider/core/config/__init__.py
+-rw-r--r--   0        0        0     1235 2024-01-23 23:46:30.499197 pygpt_net-2.2.2/src/pygpt_net/provider/core/config/base.py
+-rwxr-xr-x   0        0        0     5017 2024-04-11 01:27:21.134184 pygpt_net-2.2.2/src/pygpt_net/provider/core/config/json_file.py
+-rwxr-xr-x   0        0        0    75723 2024-04-29 05:51:11.644212 pygpt_net-2.2.2/src/pygpt_net/provider/core/config/patch.py
+-rw-r--r--   0        0        0      488 2024-01-23 23:46:30.499197 pygpt_net-2.2.2/src/pygpt_net/provider/core/ctx/__init__.py
+-rw-r--r--   0        0        0     2577 2024-04-17 05:13:33.075416 pygpt_net-2.2.2/src/pygpt_net/provider/core/ctx/base.py
+-rw-r--r--   0        0        0     9171 2024-04-17 05:13:33.075416 pygpt_net-2.2.2/src/pygpt_net/provider/core/ctx/db_sqlite/__init__.py
+-rw-r--r--   0        0        0     3101 2024-01-23 23:46:30.499197 pygpt_net-2.2.2/src/pygpt_net/provider/core/ctx/db_sqlite/patch.py
+-rw-r--r--   0        0        0    31650 2024-04-17 05:13:33.075416 pygpt_net-2.2.2/src/pygpt_net/provider/core/ctx/db_sqlite/storage.py
+-rw-r--r--   0        0        0     7644 2024-04-10 01:07:30.188635 pygpt_net-2.2.2/src/pygpt_net/provider/core/ctx/db_sqlite/utils.py
+-rw-r--r--   0        0        0    11665 2024-01-23 23:46:30.503197 pygpt_net-2.2.2/src/pygpt_net/provider/core/ctx/json_file.py
+-rw-r--r--   0        0        0      488 2024-01-23 23:46:30.503197 pygpt_net-2.2.2/src/pygpt_net/provider/core/history/__init__.py
+-rw-r--r--   0        0        0      863 2024-01-23 23:46:30.503197 pygpt_net-2.2.2/src/pygpt_net/provider/core/history/base.py
+-rw-r--r--   0        0        0      837 2024-01-23 23:46:30.503197 pygpt_net-2.2.2/src/pygpt_net/provider/core/history/patch.py
+-rw-r--r--   0        0        0     2969 2024-01-23 23:46:30.503197 pygpt_net-2.2.2/src/pygpt_net/provider/core/history/txt_file.py
+-rw-r--r--   0        0        0      488 2024-01-23 23:46:30.503197 pygpt_net-2.2.2/src/pygpt_net/provider/core/index/__init__.py
+-rw-r--r--   0        0        0     2875 2024-03-07 01:04:26.445956 pygpt_net-2.2.2/src/pygpt_net/provider/core/index/base.py
+-rw-r--r--   0        0        0     8502 2024-03-07 01:04:26.445956 pygpt_net-2.2.2/src/pygpt_net/provider/core/index/db_sqlite/__init__.py
+-rw-r--r--   0        0        0     2972 2024-02-23 06:06:25.510176 pygpt_net-2.2.2/src/pygpt_net/provider/core/index/db_sqlite/patch.py
+-rw-r--r--   0        0        0    17470 2024-03-07 01:04:26.445956 pygpt_net-2.2.2/src/pygpt_net/provider/core/index/db_sqlite/storage.py
+-rw-r--r--   0        0        0      934 2024-03-07 01:04:26.445956 pygpt_net-2.2.2/src/pygpt_net/provider/core/index/db_sqlite/utils.py
+-rw-r--r--   0        0        0     6615 2024-02-23 01:50:39.606418 pygpt_net-2.2.2/src/pygpt_net/provider/core/index/json_file.py
+-rw-r--r--   0        0        0      837 2024-01-23 23:46:30.503197 pygpt_net-2.2.2/src/pygpt_net/provider/core/index/patch.py
+-rw-r--r--   0        0        0      488 2024-01-23 23:46:30.503197 pygpt_net-2.2.2/src/pygpt_net/provider/core/mode/__init__.py
+-rw-r--r--   0        0        0     1062 2024-01-23 23:46:30.503197 pygpt_net-2.2.2/src/pygpt_net/provider/core/mode/base.py
+-rw-r--r--   0        0        0     4142 2024-01-23 23:46:30.503197 pygpt_net-2.2.2/src/pygpt_net/provider/core/mode/json_file.py
+-rw-r--r--   0        0        0      837 2024-01-23 23:46:30.503197 pygpt_net-2.2.2/src/pygpt_net/provider/core/mode/patch.py
+-rw-r--r--   0        0        0      488 2024-01-23 23:46:30.503197 pygpt_net-2.2.2/src/pygpt_net/provider/core/model/__init__.py
+-rw-r--r--   0        0        0     1246 2024-01-23 23:46:30.503197 pygpt_net-2.2.2/src/pygpt_net/provider/core/model/base.py
+-rw-r--r--   0        0        0     6231 2024-01-23 23:46:30.503197 pygpt_net-2.2.2/src/pygpt_net/provider/core/model/json_file.py
+-rw-r--r--   0        0        0     9769 2024-04-11 20:50:24.193030 pygpt_net-2.2.2/src/pygpt_net/provider/core/model/patch.py
+-rw-r--r--   0        0        0      488 2024-01-23 23:46:30.503197 pygpt_net-2.2.2/src/pygpt_net/provider/core/notepad/__init__.py
+-rw-r--r--   0        0        0     1262 2024-01-23 23:46:30.503197 pygpt_net-2.2.2/src/pygpt_net/provider/core/notepad/base.py
+-rw-r--r--   0        0        0     3044 2024-01-23 23:46:30.503197 pygpt_net-2.2.2/src/pygpt_net/provider/core/notepad/db_sqlite/__init__.py
+-rw-r--r--   0        0        0     2805 2024-01-23 23:46:30.503197 pygpt_net-2.2.2/src/pygpt_net/provider/core/notepad/db_sqlite/patch.py
+-rw-r--r--   0        0        0     7263 2024-01-23 23:46:30.503197 pygpt_net-2.2.2/src/pygpt_net/provider/core/notepad/db_sqlite/storage.py
+-rw-r--r--   0        0        0     7555 2024-01-23 23:46:30.503197 pygpt_net-2.2.2/src/pygpt_net/provider/core/notepad/json_file.py
+-rw-r--r--   0        0        0      488 2024-03-07 01:04:26.445956 pygpt_net-2.2.2/src/pygpt_net/provider/core/plugin_preset/__init__.py
+-rw-r--r--   0        0        0      987 2024-03-07 01:04:26.445956 pygpt_net-2.2.2/src/pygpt_net/provider/core/plugin_preset/base.py
+-rwxr-xr-x   0        0        0     3198 2024-03-07 01:04:26.445956 pygpt_net-2.2.2/src/pygpt_net/provider/core/plugin_preset/json_file.py
+-rwxr-xr-x   0        0        0     1766 2024-03-07 01:04:26.445956 pygpt_net-2.2.2/src/pygpt_net/provider/core/plugin_preset/patch.py
+-rwxr-xr-x   0        0        0      488 2024-01-23 23:46:30.503197 pygpt_net-2.2.2/src/pygpt_net/provider/core/preset/__init__.py
+-rwxr-xr-x   0        0        0     1300 2024-02-01 01:48:09.374583 pygpt_net-2.2.2/src/pygpt_net/provider/core/preset/base.py
+-rwxr-xr-x   0        0        0     7887 2024-02-15 05:07:04.122540 pygpt_net-2.2.2/src/pygpt_net/provider/core/preset/json_file.py
+-rw-r--r--   0        0        0     3166 2024-01-23 23:46:30.503197 pygpt_net-2.2.2/src/pygpt_net/provider/core/preset/patch.py
+-rw-r--r--   0        0        0     6961 2024-03-08 00:36:17.343108 pygpt_net-2.2.2/src/pygpt_net/provider/gpt/__init__.py
+-rw-r--r--   0        0        0    26543 2024-04-26 21:55:50.679597 pygpt_net-2.2.2/src/pygpt_net/provider/gpt/assistants.py
+-rw-r--r--   0        0        0     5763 2024-03-08 00:03:22.338417 pygpt_net-2.2.2/src/pygpt_net/provider/gpt/chat.py
+-rw-r--r--   0        0        0     5354 2024-03-09 21:41:28.193853 pygpt_net-2.2.2/src/pygpt_net/provider/gpt/completion.py
+-rw-r--r--   0        0        0     7903 2024-03-17 13:18:45.662349 pygpt_net-2.2.2/src/pygpt_net/provider/gpt/image.py
+-rw-r--r--   0        0        0     1848 2024-03-17 13:18:45.662349 pygpt_net-2.2.2/src/pygpt_net/provider/gpt/summarizer.py
+-rw-r--r--   0        0        0     7341 2024-03-12 21:25:35.838043 pygpt_net-2.2.2/src/pygpt_net/provider/gpt/vision.py
+-rw-r--r--   0        0        0        0 2024-02-20 19:10:03.189314 pygpt_net-2.2.2/src/pygpt_net/provider/gpt/worker/__init__.py
+-rw-r--r--   0        0        0    19981 2024-04-29 05:51:11.644212 pygpt_net-2.2.2/src/pygpt_net/provider/gpt/worker/assistants.py
+-rw-r--r--   0        0        0    10157 2024-04-27 07:58:32.750704 pygpt_net-2.2.2/src/pygpt_net/provider/gpt/worker/importer.py
+-rwxr-xr-x   0        0        0        0 2024-01-27 21:42:30.960980 pygpt_net-2.2.2/src/pygpt_net/provider/llms/__init__.py
+-rwxr-xr-x   0        0        0     1641 2024-01-27 21:42:30.960980 pygpt_net-2.2.2/src/pygpt_net/provider/llms/anthropic.py
+-rwxr-xr-x   0        0        0     2800 2024-03-13 15:08:01.569797 pygpt_net-2.2.2/src/pygpt_net/provider/llms/azure_openai.py
+-rw-r--r--   0        0        0     3940 2024-03-15 15:31:21.790122 pygpt_net-2.2.2/src/pygpt_net/provider/llms/base.py
+-rwxr-xr-x   0        0        0     1535 2024-01-27 21:42:30.960980 pygpt_net-2.2.2/src/pygpt_net/provider/llms/hugging_face.py
+-rwxr-xr-x   0        0        0     1643 2024-01-27 21:42:30.960980 pygpt_net-2.2.2/src/pygpt_net/provider/llms/llama.py
+-rwxr-xr-x   0        0        0     1517 2024-01-27 21:42:30.960980 pygpt_net-2.2.2/src/pygpt_net/provider/llms/ollama.py
+-rwxr-xr-x   0        0        0     2727 2024-03-13 15:08:01.569797 pygpt_net-2.2.2/src/pygpt_net/provider/llms/openai.py
+-rw-r--r--   0        0        0        0 2024-01-23 23:46:30.503197 pygpt_net-2.2.2/src/pygpt_net/provider/loaders/__init__.py
+-rw-r--r--   0        0        0     2515 2024-04-17 01:35:30.426055 pygpt_net-2.2.2/src/pygpt_net/provider/loaders/base.py
+-rw-r--r--   0        0        0     1258 2024-04-17 01:35:30.426055 pygpt_net-2.2.2/src/pygpt_net/provider/loaders/file_csv.py
+-rw-r--r--   0        0        0     1032 2024-02-29 03:07:51.278132 pygpt_net-2.2.2/src/pygpt_net/provider/loaders/file_docx.py
+-rw-r--r--   0        0        0     1022 2024-02-29 03:07:51.278132 pygpt_net-2.2.2/src/pygpt_net/provider/loaders/file_epub.py
+-rw-r--r--   0        0        0     1032 2024-02-28 03:58:59.309445 pygpt_net-2.2.2/src/pygpt_net/provider/loaders/file_excel.py
+-rw-r--r--   0        0        0     1268 2024-04-17 01:35:30.426055 pygpt_net-2.2.2/src/pygpt_net/provider/loaders/file_html.py
+-rw-r--r--   0        0        0     1923 2024-04-17 01:35:30.426055 pygpt_net-2.2.2/src/pygpt_net/provider/loaders/file_image_vision.py
+-rw-r--r--   0        0        0     1284 2024-04-17 01:35:30.426055 pygpt_net-2.2.2/src/pygpt_net/provider/loaders/file_ipynb.py
+-rw-r--r--   0        0        0      996 2024-02-28 03:58:59.309445 pygpt_net-2.2.2/src/pygpt_net/provider/loaders/file_json.py
+-rw-r--r--   0        0        0     1292 2024-04-17 01:35:30.426055 pygpt_net-2.2.2/src/pygpt_net/provider/loaders/file_markdown.py
+-rw-r--r--   0        0        0     1214 2024-04-17 01:35:30.426055 pygpt_net-2.2.2/src/pygpt_net/provider/loaders/file_pdf.py
+-rw-r--r--   0        0        0     1832 2024-04-17 01:35:30.426055 pygpt_net-2.2.2/src/pygpt_net/provider/loaders/file_video_audio.py
+-rw-r--r--   0        0        0     1196 2024-04-17 01:35:30.426055 pygpt_net-2.2.2/src/pygpt_net/provider/loaders/file_xml.py
+-rw-r--r--   0        0        0        0 2024-01-27 21:42:30.960980 pygpt_net-2.2.2/src/pygpt_net/provider/loaders/hub/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-01 17:40:19.825274 pygpt_net-2.2.2/src/pygpt_net/provider/loaders/hub/bitbucket/__init__.py
+-rw-r--r--   0        0        0     6194 2024-03-01 17:40:19.825274 pygpt_net-2.2.2/src/pygpt_net/provider/loaders/hub/bitbucket/repo.py
+-rw-r--r--   0        0        0        0 2024-03-01 17:40:19.825274 pygpt_net-2.2.2/src/pygpt_net/provider/loaders/hub/chatgpt_retrieval/__init__.py
+-rw-r--r--   0        0        0     2460 2024-03-01 17:40:19.825274 pygpt_net-2.2.2/src/pygpt_net/provider/loaders/hub/chatgpt_retrieval/base.py
+-rw-r--r--   0        0        0        0 2024-03-01 17:40:19.825274 pygpt_net-2.2.2/src/pygpt_net/provider/loaders/hub/database/__init__.py
+-rw-r--r--   0        0        0     4228 2024-03-01 17:40:19.825274 pygpt_net-2.2.2/src/pygpt_net/provider/loaders/hub/database/base.py
+-rw-r--r--   0        0        0        0 2024-03-01 17:40:19.825274 pygpt_net-2.2.2/src/pygpt_net/provider/loaders/hub/github/__init__.py
+-rw-r--r--   0        0        0     4204 2024-03-01 17:40:19.825274 pygpt_net-2.2.2/src/pygpt_net/provider/loaders/hub/github/issues.py
+-rw-r--r--   0        0        0     3550 2024-03-01 17:40:19.825274 pygpt_net-2.2.2/src/pygpt_net/provider/loaders/hub/github/repo.py
+-rw-r--r--   0        0        0        0 2024-03-01 03:17:53.457929 pygpt_net-2.2.2/src/pygpt_net/provider/loaders/hub/google/__init__.py
+-rw-r--r--   0        0        0     2658 2024-03-01 03:17:53.457929 pygpt_net-2.2.2/src/pygpt_net/provider/loaders/hub/google/calendar.py
+-rw-r--r--   0        0        0     5370 2024-03-01 03:17:53.457929 pygpt_net-2.2.2/src/pygpt_net/provider/loaders/hub/google/docs.py
+-rw-r--r--   0        0        0     6772 2024-03-01 03:17:53.457929 pygpt_net-2.2.2/src/pygpt_net/provider/loaders/hub/google/gmail.py
+-rw-r--r--   0        0        0     1633 2024-03-01 03:17:53.457929 pygpt_net-2.2.2/src/pygpt_net/provider/loaders/hub/google/keep.py
+-rw-r--r--   0        0        0     5282 2024-03-01 03:17:53.457929 pygpt_net-2.2.2/src/pygpt_net/provider/loaders/hub/google/sheets.py
+-rw-r--r--   0        0        0        0 2024-03-01 03:17:53.457929 pygpt_net-2.2.2/src/pygpt_net/provider/loaders/hub/image_vision/__init__.py
+-rw-r--r--   0        0        0     6940 2024-03-01 03:17:53.457929 pygpt_net-2.2.2/src/pygpt_net/provider/loaders/hub/image_vision/base.py
+-rw-r--r--   0        0        0        0 2024-01-27 21:42:30.964980 pygpt_net-2.2.2/src/pygpt_net/provider/loaders/hub/json/__init__.py
+-rw-r--r--   0        0        0     3862 2024-02-29 03:07:51.278132 pygpt_net-2.2.2/src/pygpt_net/provider/loaders/hub/json/base.py
+-rw-r--r--   0        0        0        0 2024-01-27 21:42:30.964980 pygpt_net-2.2.2/src/pygpt_net/provider/loaders/hub/pandas_excel/__init__.py
+-rw-r--r--   0        0        0     3940 2024-02-29 03:07:51.278132 pygpt_net-2.2.2/src/pygpt_net/provider/loaders/hub/pandas_excel/base.py
+-rw-r--r--   0        0        0        0 2024-01-27 21:42:30.964980 pygpt_net-2.2.2/src/pygpt_net/provider/loaders/hub/simple_csv/__init__.py
+-rw-r--r--   0        0        0     1481 2024-02-29 03:07:51.278132 pygpt_net-2.2.2/src/pygpt_net/provider/loaders/hub/simple_csv/base.py
+-rw-r--r--   0        0        0        0 2024-03-01 03:17:53.457929 pygpt_net-2.2.2/src/pygpt_net/provider/loaders/hub/video_audio/__init__.py
+-rw-r--r--   0        0        0     4960 2024-03-01 03:17:53.457929 pygpt_net-2.2.2/src/pygpt_net/provider/loaders/hub/video_audio/base.py
+-rw-r--r--   0        0        0        0 2024-02-27 05:21:39.771084 pygpt_net-2.2.2/src/pygpt_net/provider/loaders/hub/web_page/__init__.py
+-rw-r--r--   0        0        0      556 2024-02-29 03:07:51.278132 pygpt_net-2.2.2/src/pygpt_net/provider/loaders/hub/web_page/base.py
+-rw-r--r--   0        0        0        0 2024-02-27 05:21:39.771084 pygpt_net-2.2.2/src/pygpt_net/provider/loaders/hub/yt/__init__.py
+-rw-r--r--   0        0        0     2427 2024-02-29 03:07:51.278132 pygpt_net-2.2.2/src/pygpt_net/provider/loaders/hub/yt/base.py
+-rw-r--r--   0        0        0      545 2024-02-27 05:21:39.771084 pygpt_net-2.2.2/src/pygpt_net/provider/loaders/hub/yt/utils.py
+-rw-r--r--   0        0        0     3626 2024-04-17 01:35:30.426055 pygpt_net-2.2.2/src/pygpt_net/provider/loaders/web_bitbucket.py
+-rw-r--r--   0        0        0     2580 2024-04-17 01:35:30.426055 pygpt_net-2.2.2/src/pygpt_net/provider/loaders/web_chatgpt_retrieval.py
+-rw-r--r--   0        0        0     2834 2024-04-17 01:35:30.426055 pygpt_net-2.2.2/src/pygpt_net/provider/loaders/web_database.py
+-rw-r--r--   0        0        0     3832 2024-04-17 01:35:30.426055 pygpt_net-2.2.2/src/pygpt_net/provider/loaders/web_github_issues.py
+-rw-r--r--   0        0        0     4377 2024-04-17 01:35:30.426055 pygpt_net-2.2.2/src/pygpt_net/provider/loaders/web_github_repo.py
+-rw-r--r--   0        0        0     2834 2024-04-17 01:35:30.430055 pygpt_net-2.2.2/src/pygpt_net/provider/loaders/web_google_calendar.py
+-rw-r--r--   0        0        0     2480 2024-04-17 01:35:30.430055 pygpt_net-2.2.2/src/pygpt_net/provider/loaders/web_google_docs.py
+-rw-r--r--   0        0        0     3582 2024-04-17 01:35:30.430055 pygpt_net-2.2.2/src/pygpt_net/provider/loaders/web_google_drive.py
+-rw-r--r--   0        0        0     2710 2024-04-17 01:35:30.430055 pygpt_net-2.2.2/src/pygpt_net/provider/loaders/web_google_gmail.py
+-rw-r--r--   0        0        0     2412 2024-04-17 01:35:30.430055 pygpt_net-2.2.2/src/pygpt_net/provider/loaders/web_google_keep.py
+-rw-r--r--   0        0        0     2590 2024-04-17 01:35:30.430055 pygpt_net-2.2.2/src/pygpt_net/provider/loaders/web_google_sheets.py
+-rw-r--r--   0        0        0     4004 2024-04-17 01:35:30.430055 pygpt_net-2.2.2/src/pygpt_net/provider/loaders/web_microsoft_onedrive.py
+-rw-r--r--   0        0        0     1572 2024-03-12 06:49:17.168786 pygpt_net-2.2.2/src/pygpt_net/provider/loaders/web_page.py
+-rw-r--r--   0        0        0     1584 2024-03-12 06:49:17.172787 pygpt_net-2.2.2/src/pygpt_net/provider/loaders/web_rss.py
+-rw-r--r--   0        0        0     1853 2024-04-17 01:35:30.430055 pygpt_net-2.2.2/src/pygpt_net/provider/loaders/web_sitemap.py
+-rw-r--r--   0        0        0     2831 2024-04-17 01:35:30.430055 pygpt_net-2.2.2/src/pygpt_net/provider/loaders/web_twitter.py
+-rw-r--r--   0        0        0     1617 2024-03-12 06:49:17.172787 pygpt_net-2.2.2/src/pygpt_net/provider/loaders/web_yt.py
+-rw-r--r--   0        0        0     5976 2024-03-08 22:55:56.889343 pygpt_net-2.2.2/src/pygpt_net/provider/vector_stores/__init__.py
+-rw-r--r--   0        0        0     3791 2024-03-11 03:15:21.875594 pygpt_net-2.2.2/src/pygpt_net/provider/vector_stores/base.py
+-rwxr-xr-x   0        0        0     3036 2024-03-11 03:15:21.875594 pygpt_net-2.2.2/src/pygpt_net/provider/vector_stores/chroma.py
+-rw-r--r--   0        0        0     3016 2024-03-11 03:15:21.875594 pygpt_net-2.2.2/src/pygpt_net/provider/vector_stores/elasticsearch.py
+-rw-r--r--   0        0        0     5041 2024-03-11 03:15:21.875594 pygpt_net-2.2.2/src/pygpt_net/provider/vector_stores/pinecode.py
+-rw-r--r--   0        0        0     3047 2024-03-11 03:15:21.875594 pygpt_net-2.2.2/src/pygpt_net/provider/vector_stores/redis.py
+-rw-r--r--   0        0        0     2455 2024-03-11 03:15:21.875594 pygpt_net-2.2.2/src/pygpt_net/provider/vector_stores/simple.py
+-rw-r--r--   0        0        0     4322 2024-03-11 03:15:21.875594 pygpt_net-2.2.2/src/pygpt_net/provider/vector_stores/temp.py
+-rw-r--r--   0        0        0      488 2024-02-24 01:55:58.449111 pygpt_net-2.2.2/src/pygpt_net/provider/web/__init__.py
+-rw-r--r--   0        0        0     1994 2024-02-27 05:21:39.771084 pygpt_net-2.2.2/src/pygpt_net/provider/web/base.py
+-rw-r--r--   0        0        0     4646 2024-02-25 00:27:02.862945 pygpt_net-2.2.2/src/pygpt_net/provider/web/google_custom_search.py
+-rw-r--r--   0        0        0     4104 2024-02-25 00:27:02.862945 pygpt_net-2.2.2/src/pygpt_net/provider/web/microsoft_bing.py
+-rw-r--r--   0        0        0     3917 2024-04-19 00:32:20.498428 pygpt_net-2.2.2/src/pygpt_net/tools/__init__.py
+-rwxr-xr-x   0        0        0     9791 2024-03-26 17:12:51.294309 pygpt_net-2.2.2/src/pygpt_net/tools/audio_transcriber/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-26 17:12:51.294309 pygpt_net-2.2.2/src/pygpt_net/tools/audio_transcriber/ui/__init__.py
+-rw-r--r--   0        0        0     5666 2024-03-26 17:12:51.294309 pygpt_net-2.2.2/src/pygpt_net/tools/audio_transcriber/ui/dialogs.py
+-rw-r--r--   0        0        0     2116 2024-04-19 00:32:20.498428 pygpt_net-2.2.2/src/pygpt_net/tools/base.py
+-rwxr-xr-x   0        0        0    11427 2024-04-19 00:32:20.498428 pygpt_net-2.2.2/src/pygpt_net/tools/code_interpreter/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-26 17:12:51.294309 pygpt_net-2.2.2/src/pygpt_net/tools/code_interpreter/ui/__init__.py
+-rw-r--r--   0        0        0     6580 2024-03-26 17:12:51.294309 pygpt_net-2.2.2/src/pygpt_net/tools/code_interpreter/ui/dialogs.py
+-rw-r--r--   0        0        0     3518 2024-03-26 17:12:51.294309 pygpt_net-2.2.2/src/pygpt_net/tools/code_interpreter/ui/widgets.py
+-rwxr-xr-x   0        0        0     9063 2024-04-14 16:40:07.849541 pygpt_net-2.2.2/src/pygpt_net/tools/image_viewer/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-26 17:12:51.294309 pygpt_net-2.2.2/src/pygpt_net/tools/image_viewer/ui/__init__.py
+-rw-r--r--   0        0        0     4962 2024-03-26 17:12:51.294309 pygpt_net-2.2.2/src/pygpt_net/tools/image_viewer/ui/dialogs.py
+-rwxr-xr-x   0        0        0    18833 2024-04-19 00:32:20.498428 pygpt_net-2.2.2/src/pygpt_net/tools/indexer/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-17 01:35:30.430055 pygpt_net-2.2.2/src/pygpt_net/tools/indexer/ui/__init__.py
+-rw-r--r--   0        0        0     1438 2024-04-17 01:35:30.430055 pygpt_net-2.2.2/src/pygpt_net/tools/indexer/ui/browse.py
+-rw-r--r--   0        0        0     4355 2024-04-17 01:35:30.430055 pygpt_net-2.2.2/src/pygpt_net/tools/indexer/ui/ctx.py
+-rw-r--r--   0        0        0     7985 2024-04-17 01:35:30.430055 pygpt_net-2.2.2/src/pygpt_net/tools/indexer/ui/dialogs.py
+-rw-r--r--   0        0        0     4034 2024-04-17 01:35:30.430055 pygpt_net-2.2.2/src/pygpt_net/tools/indexer/ui/files.py
+-rw-r--r--   0        0        0    10477 2024-04-17 01:35:30.430055 pygpt_net-2.2.2/src/pygpt_net/tools/indexer/ui/web.py
+-rw-r--r--   0        0        0     3562 2024-04-17 01:35:30.430055 pygpt_net-2.2.2/src/pygpt_net/tools/indexer/ui/widgets.py
+-rwxr-xr-x   0        0        0     6028 2024-03-26 17:12:51.294309 pygpt_net-2.2.2/src/pygpt_net/tools/media_player/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-26 17:12:51.294309 pygpt_net-2.2.2/src/pygpt_net/tools/media_player/ui/__init__.py
+-rw-r--r--   0        0        0     3590 2024-03-26 17:12:51.294309 pygpt_net-2.2.2/src/pygpt_net/tools/media_player/ui/dialogs.py
+-rw-r--r--   0        0        0    15702 2024-03-26 17:12:51.294309 pygpt_net-2.2.2/src/pygpt_net/tools/media_player/ui/widgets.py
+-rw-r--r--   0        0        0     8018 2024-04-14 16:40:07.849541 pygpt_net-2.2.2/src/pygpt_net/tools/text_editor/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-26 17:12:51.294309 pygpt_net-2.2.2/src/pygpt_net/tools/text_editor/ui/__init__.py
+-rw-r--r--   0        0        0     2906 2024-04-11 00:43:06.922864 pygpt_net-2.2.2/src/pygpt_net/tools/text_editor/ui/dialogs.py
+-rw-r--r--   0        0        0     2754 2024-04-11 03:43:59.058733 pygpt_net-2.2.2/src/pygpt_net/tools/text_editor/ui/widgets.py
+-rwxr-xr-x   0        0        0     6639 2024-04-10 01:07:30.188635 pygpt_net-2.2.2/src/pygpt_net/ui/__init__.py
+-rw-r--r--   0        0        0        0 2024-01-08 20:36:28.054492 pygpt_net-2.2.2/src/pygpt_net/ui/base/__init__.py
+-rw-r--r--   0        0        0     9209 2024-03-11 07:32:25.337990 pygpt_net-2.2.2/src/pygpt_net/ui/base/config_dialog.py
+-rw-r--r--   0        0        0     3430 2024-03-26 17:12:51.294309 pygpt_net-2.2.2/src/pygpt_net/ui/base/context_menu.py
+-rwxr-xr-x   0        0        0      488 2023-12-28 18:11:19.000000 pygpt_net-2.2.2/src/pygpt_net/ui/dialog/__init__.py
+-rwxr-xr-x   0        0        0     5730 2024-04-11 20:50:24.193030 pygpt_net-2.2.2/src/pygpt_net/ui/dialog/about.py
+-rwxr-xr-x   0        0        0     5140 2024-03-26 17:12:51.294309 pygpt_net-2.2.2/src/pygpt_net/ui/dialog/applog.py
+-rwxr-xr-x   0        0        0     6480 2024-04-28 06:16:26.324027 pygpt_net-2.2.2/src/pygpt_net/ui/dialog/assistant.py
+-rw-r--r--   0        0        0    17707 2024-04-27 07:58:32.754704 pygpt_net-2.2.2/src/pygpt_net/ui/dialog/assistant_store.py
+-rwxr-xr-x   0        0        0     1765 2024-03-18 02:45:45.661442 pygpt_net-2.2.2/src/pygpt_net/ui/dialog/changelog.py
+-rw-r--r--   0        0        0      973 2024-01-28 19:32:28.495073 pygpt_net-2.2.2/src/pygpt_net/ui/dialog/create.py
+-rw-r--r--   0        0        0    18520 2024-04-17 01:35:30.430055 pygpt_net-2.2.2/src/pygpt_net/ui/dialog/db.py
+-rwxr-xr-x   0        0        0     1864 2024-03-18 04:54:07.637826 pygpt_net-2.2.2/src/pygpt_net/ui/dialog/debug.py
+-rw-r--r--   0        0        0     5835 2024-03-12 06:49:17.172787 pygpt_net-2.2.2/src/pygpt_net/ui/dialog/dictionary.py
+-rwxr-xr-x   0        0        0     2926 2024-04-10 01:07:30.188635 pygpt_net-2.2.2/src/pygpt_net/ui/dialog/editor.py
+-rw-r--r--   0        0        0      957 2024-04-08 04:19:15.433912 pygpt_net-2.2.2/src/pygpt_net/ui/dialog/find.py
+-rwxr-xr-x   0        0        0     2876 2024-03-26 17:12:51.294309 pygpt_net-2.2.2/src/pygpt_net/ui/dialog/image.py
+-rwxr-xr-x   0        0        0     2272 2024-03-18 02:45:42.817463 pygpt_net-2.2.2/src/pygpt_net/ui/dialog/license.py
+-rwxr-xr-x   0        0        0     1823 2024-03-26 17:12:51.294309 pygpt_net-2.2.2/src/pygpt_net/ui/dialog/logger.py
+-rw-r--r--   0        0        0    13166 2024-03-10 12:05:00.639613 pygpt_net-2.2.2/src/pygpt_net/ui/dialog/models.py
+-rwxr-xr-x   0        0        0    20679 2024-03-12 06:49:17.172787 pygpt_net-2.2.2/src/pygpt_net/ui/dialog/plugins.py
+-rwxr-xr-x   0        0        0     6644 2024-02-15 05:07:04.122540 pygpt_net-2.2.2/src/pygpt_net/ui/dialog/preset.py
+-rw-r--r--   0        0        0     3796 2024-03-07 01:04:26.445956 pygpt_net-2.2.2/src/pygpt_net/ui/dialog/preset_plugins.py
+-rw-r--r--   0        0        0     4105 2024-04-10 01:07:30.188635 pygpt_net-2.2.2/src/pygpt_net/ui/dialog/profile.py
+-rwxr-xr-x   0        0        0      973 2024-01-28 19:32:28.495073 pygpt_net-2.2.2/src/pygpt_net/ui/dialog/rename.py
+-rwxr-xr-x   0        0        0    15113 2024-03-10 12:05:00.639613 pygpt_net-2.2.2/src/pygpt_net/ui/dialog/settings.py
+-rw-r--r--   0        0        0      954 2024-02-26 22:26:37.124323 pygpt_net-2.2.2/src/pygpt_net/ui/dialog/snap.py
+-rwxr-xr-x   0        0        0     2436 2024-02-25 05:55:37.513980 pygpt_net-2.2.2/src/pygpt_net/ui/dialog/start.py
+-rwxr-xr-x   0        0        0      842 2023-12-28 18:11:19.000000 pygpt_net-2.2.2/src/pygpt_net/ui/dialog/update.py
+-rw-r--r--   0        0        0     4275 2024-03-26 17:12:51.294309 pygpt_net-2.2.2/src/pygpt_net/ui/dialog/workdir.py
+-rwxr-xr-x   0        0        0     9009 2024-04-26 21:55:50.679597 pygpt_net-2.2.2/src/pygpt_net/ui/dialogs.py
+-rwxr-xr-x   0        0        0      488 2023-12-28 21:20:40.362230 pygpt_net-2.2.2/src/pygpt_net/ui/layout/__init__.py
+-rwxr-xr-x   0        0        0     1535 2024-04-09 20:34:52.308546 pygpt_net-2.2.2/src/pygpt_net/ui/layout/chat/__init__.py
+-rwxr-xr-x   0        0        0     5518 2024-04-14 20:50:29.556142 pygpt_net-2.2.2/src/pygpt_net/ui/layout/chat/attachments.py
+-rwxr-xr-x   0        0        0     5356 2024-04-27 07:58:32.754704 pygpt_net-2.2.2/src/pygpt_net/ui/layout/chat/attachments_uploaded.py
+-rw-r--r--   0        0        0     5996 2024-04-10 01:07:30.188635 pygpt_net-2.2.2/src/pygpt_net/ui/layout/chat/calendar.py
+-rwxr-xr-x   0        0        0     9885 2024-04-09 20:35:55.668463 pygpt_net-2.2.2/src/pygpt_net/ui/layout/chat/input.py
+-rwxr-xr-x   0        0        0    18656 2024-01-01 00:17:57.553256 pygpt_net-2.2.2/src/pygpt_net/ui/layout/chat/markdown.py
+-rwxr-xr-x   0        0        0    10452 2024-04-21 18:06:27.128064 pygpt_net-2.2.2/src/pygpt_net/ui/layout/chat/output.py
+-rw-r--r--   0        0        0     5199 2024-02-17 21:22:47.345663 pygpt_net-2.2.2/src/pygpt_net/ui/layout/chat/painter.py
+-rwxr-xr-x   0        0        0     1697 2024-01-27 21:42:30.964980 pygpt_net-2.2.2/src/pygpt_net/ui/layout/ctx/__init__.py
+-rwxr-xr-x   0        0        0     6648 2024-04-21 19:42:04.971470 pygpt_net-2.2.2/src/pygpt_net/ui/layout/ctx/ctx_list.py
+-rwxr-xr-x   0        0        0     1441 2024-01-07 09:35:02.638810 pygpt_net-2.2.2/src/pygpt_net/ui/layout/ctx/search_input.py
+-rwxr-xr-x   0        0        0     1068 2023-12-31 01:26:09.880264 pygpt_net-2.2.2/src/pygpt_net/ui/layout/ctx/video.py
+-rwxr-xr-x   0        0        0     1405 2024-01-31 15:19:17.742029 pygpt_net-2.2.2/src/pygpt_net/ui/layout/status.py
+-rwxr-xr-x   0        0        0     3477 2024-04-27 14:05:11.727541 pygpt_net-2.2.2/src/pygpt_net/ui/layout/toolbox/__init__.py
+-rw-r--r--   0        0        0     2378 2024-01-30 17:23:19.901578 pygpt_net-2.2.2/src/pygpt_net/ui/layout/toolbox/agent.py
+-rwxr-xr-x   0        0        0     4427 2024-04-27 07:58:32.754704 pygpt_net-2.2.2/src/pygpt_net/ui/layout/toolbox/assistants.py
+-rwxr-xr-x   0        0        0     4254 2024-02-29 03:07:51.278132 pygpt_net-2.2.2/src/pygpt_net/ui/layout/toolbox/footer.py
+-rwxr-xr-x   0        0        0     2382 2024-01-21 16:42:14.672394 pygpt_net-2.2.2/src/pygpt_net/ui/layout/toolbox/image.py
+-rw-r--r--   0        0        0     6999 2024-04-27 14:05:11.727541 pygpt_net-2.2.2/src/pygpt_net/ui/layout/toolbox/indexes.py
+-rwxr-xr-x   0        0        0     3169 2024-02-21 03:55:24.484309 pygpt_net-2.2.2/src/pygpt_net/ui/layout/toolbox/mode.py
+-rwxr-xr-x   0        0        0     3067 2024-02-21 03:55:24.484309 pygpt_net-2.2.2/src/pygpt_net/ui/layout/toolbox/model.py
+-rwxr-xr-x   0        0        0     4125 2024-03-15 15:31:21.790122 pygpt_net-2.2.2/src/pygpt_net/ui/layout/toolbox/presets.py
+-rwxr-xr-x   0        0        0     3242 2024-03-15 15:31:21.790122 pygpt_net-2.2.2/src/pygpt_net/ui/layout/toolbox/prompt.py
+-rwxr-xr-x   0        0        0     2447 2023-12-31 01:26:09.000000 pygpt_net-2.2.2/src/pygpt_net/ui/layout/toolbox/vision.py
+-rw-r--r--   0        0        0     9644 2024-04-29 05:51:11.644212 pygpt_net-2.2.2/src/pygpt_net/ui/main.py
+-rw-r--r--   0        0        0     1784 2024-03-26 17:12:51.294309 pygpt_net-2.2.2/src/pygpt_net/ui/menu/__init__.py
+-rw-r--r--   0        0        0     5067 2024-04-19 00:32:20.498428 pygpt_net-2.2.2/src/pygpt_net/ui/menu/about.py
+-rw-r--r--   0        0        0     1655 2024-03-20 16:01:43.283339 pygpt_net-2.2.2/src/pygpt_net/ui/menu/audio.py
+-rw-r--r--   0        0        0     7870 2024-04-21 01:33:54.247764 pygpt_net-2.2.2/src/pygpt_net/ui/menu/config.py
+-rw-r--r--   0        0        0     5185 2024-03-07 01:04:26.445956 pygpt_net-2.2.2/src/pygpt_net/ui/menu/debug.py
+-rw-r--r--   0        0        0     3356 2024-04-17 05:13:33.075416 pygpt_net-2.2.2/src/pygpt_net/ui/menu/file.py
+-rw-r--r--   0        0        0      897 2024-01-27 21:42:30.964980 pygpt_net-2.2.2/src/pygpt_net/ui/menu/lang.py
+-rw-r--r--   0        0        0     2880 2024-03-07 01:04:26.445956 pygpt_net-2.2.2/src/pygpt_net/ui/menu/plugins.py
+-rwxr-xr-x   0        0        0     3440 2024-04-24 23:37:32.616565 pygpt_net-2.2.2/src/pygpt_net/ui/menu/theme.py
+-rw-r--r--   0        0        0     1134 2024-03-26 17:12:51.298308 pygpt_net-2.2.2/src/pygpt_net/ui/menu/tools.py
+-rw-r--r--   0        0        0     2026 2024-03-20 16:01:43.283339 pygpt_net-2.2.2/src/pygpt_net/ui/menu/video.py
+-rw-r--r--   0        0        0     6711 2024-04-14 20:50:29.556142 pygpt_net-2.2.2/src/pygpt_net/ui/tray.py
+-rwxr-xr-x   0        0        0      488 2023-12-28 18:11:19.000000 pygpt_net-2.2.2/src/pygpt_net/ui/widget/__init__.py
+-rwxr-xr-x   0        0        0      488 2023-12-28 21:20:40.362230 pygpt_net-2.2.2/src/pygpt_net/ui/widget/audio/__init__.py
+-rwxr-xr-x   0        0        0     1721 2023-12-28 21:20:40.362230 pygpt_net-2.2.2/src/pygpt_net/ui/widget/audio/input.py
+-rw-r--r--   0        0        0     2198 2024-02-29 03:07:51.278132 pygpt_net-2.2.2/src/pygpt_net/ui/widget/audio/input_button.py
+-rwxr-xr-x   0        0        0     1586 2023-12-28 21:20:40.362230 pygpt_net-2.2.2/src/pygpt_net/ui/widget/audio/output.py
+-rw-r--r--   0        0        0        0 2024-01-06 03:25:04.270157 pygpt_net-2.2.2/src/pygpt_net/ui/widget/calendar/__init__.py
+-rw-r--r--   0        0        0     8120 2024-04-27 07:58:32.754704 pygpt_net-2.2.2/src/pygpt_net/ui/widget/calendar/select.py
+-rwxr-xr-x   0        0        0      488 2023-12-28 21:20:40.362230 pygpt_net-2.2.2/src/pygpt_net/ui/widget/dialog/__init__.py
+-rwxr-xr-x   0        0        0     1429 2024-04-17 01:35:30.430055 pygpt_net-2.2.2/src/pygpt_net/ui/widget/dialog/alert.py
+-rw-r--r--   0        0        0     1502 2024-02-17 21:22:47.345663 pygpt_net-2.2.2/src/pygpt_net/ui/widget/dialog/applog.py
+-rw-r--r--   0        0        0     1712 2024-04-26 21:55:50.679597 pygpt_net-2.2.2/src/pygpt_net/ui/widget/dialog/assistant_store.py
+-rw-r--r--   0        0        0      551 2024-03-26 17:12:51.298308 pygpt_net-2.2.2/src/pygpt_net/ui/widget/dialog/audio.py
+-rwxr-xr-x   0        0        0     3802 2024-04-11 03:43:59.058733 pygpt_net-2.2.2/src/pygpt_net/ui/widget/dialog/base.py
+-rwxr-xr-x   0        0        0     2302 2024-04-12 10:08:45.275113 pygpt_net-2.2.2/src/pygpt_net/ui/widget/dialog/confirm.py
+-rw-r--r--   0        0        0     2191 2024-01-28 19:32:28.495073 pygpt_net-2.2.2/src/pygpt_net/ui/widget/dialog/create.py
+-rw-r--r--   0        0        0     1585 2024-03-07 01:04:26.445956 pygpt_net-2.2.2/src/pygpt_net/ui/widget/dialog/db.py
+-rwxr-xr-x   0        0        0     1572 2024-02-21 16:35:35.211671 pygpt_net-2.2.2/src/pygpt_net/ui/widget/dialog/debug.py
+-rwxr-xr-x   0        0        0     1749 2024-02-17 21:22:47.345663 pygpt_net-2.2.2/src/pygpt_net/ui/widget/dialog/editor.py
+-rwxr-xr-x   0        0        0     6185 2024-04-14 16:40:07.849541 pygpt_net-2.2.2/src/pygpt_net/ui/widget/dialog/editor_file.py
+-rw-r--r--   0        0        0     3242 2024-04-11 03:43:59.058733 pygpt_net-2.2.2/src/pygpt_net/ui/widget/dialog/find.py
+-rwxr-xr-x   0        0        0      816 2024-03-26 17:12:51.298308 pygpt_net-2.2.2/src/pygpt_net/ui/widget/dialog/image.py
+-rwxr-xr-x   0        0        0     1568 2024-02-17 21:22:47.345663 pygpt_net-2.2.2/src/pygpt_net/ui/widget/dialog/info.py
+-rw-r--r--   0        0        0     1717 2024-02-17 21:22:47.345663 pygpt_net-2.2.2/src/pygpt_net/ui/widget/dialog/license.py
+-rwxr-xr-x   0        0        0     1627 2024-02-17 21:22:47.345663 pygpt_net-2.2.2/src/pygpt_net/ui/widget/dialog/logger.py
+-rw-r--r--   0        0        0     1625 2024-02-17 21:22:47.345663 pygpt_net-2.2.2/src/pygpt_net/ui/widget/dialog/model.py
+-rw-r--r--   0        0        0     1694 2024-04-10 01:07:30.188635 pygpt_net-2.2.2/src/pygpt_net/ui/widget/dialog/preset_plugins.py
+-rw-r--r--   0        0        0     6686 2024-04-19 00:32:20.502428 pygpt_net-2.2.2/src/pygpt_net/ui/widget/dialog/profile.py
+-rwxr-xr-x   0        0        0     2191 2024-01-28 19:32:28.495073 pygpt_net-2.2.2/src/pygpt_net/ui/widget/dialog/rename.py
+-rwxr-xr-x   0        0        0     1614 2024-02-17 21:22:47.345663 pygpt_net-2.2.2/src/pygpt_net/ui/widget/dialog/settings.py
+-rwxr-xr-x   0        0        0     1696 2024-02-17 21:22:47.345663 pygpt_net-2.2.2/src/pygpt_net/ui/widget/dialog/settings_plugin.py
+-rw-r--r--   0        0        0     2724 2024-02-26 22:26:37.124323 pygpt_net-2.2.2/src/pygpt_net/ui/widget/dialog/snap.py
+-rwxr-xr-x   0        0        0     6789 2024-02-17 21:22:47.345663 pygpt_net-2.2.2/src/pygpt_net/ui/widget/dialog/update.py
+-rw-r--r--   0        0        0     1523 2024-03-26 17:12:51.298308 pygpt_net-2.2.2/src/pygpt_net/ui/widget/dialog/workdir.py
+-rwxr-xr-x   0        0        0      488 2024-01-11 15:56:53.277343 pygpt_net-2.2.2/src/pygpt_net/ui/widget/draw/__init__.py
+-rw-r--r--   0        0        0    10903 2024-04-12 07:23:35.946682 pygpt_net-2.2.2/src/pygpt_net/ui/widget/draw/painter.py
+-rwxr-xr-x   0        0        0      488 2023-12-28 21:20:40.362230 pygpt_net-2.2.2/src/pygpt_net/ui/widget/element/__init__.py
+-rw-r--r--   0        0        0     2854 2024-04-14 20:50:29.556142 pygpt_net-2.2.2/src/pygpt_net/ui/widget/element/button.py
+-rw-r--r--   0        0        0     2532 2024-03-07 01:04:26.445956 pygpt_net-2.2.2/src/pygpt_net/ui/widget/element/checkbox.py
+-rwxr-xr-x   0        0        0     2559 2024-01-27 21:42:30.964980 pygpt_net-2.2.2/src/pygpt_net/ui/widget/element/group.py
+-rw-r--r--   0        0        0     3789 2024-02-28 03:58:59.313445 pygpt_net-2.2.2/src/pygpt_net/ui/widget/element/labels.py
+-rwxr-xr-x   0        0        0        0 2023-12-28 21:20:40.362230 pygpt_net-2.2.2/src/pygpt_net/ui/widget/filesystem/__init__.py
+-rwxr-xr-x   0        0        0    22934 2024-04-17 01:35:30.430055 pygpt_net-2.2.2/src/pygpt_net/ui/widget/filesystem/explorer.py
+-rwxr-xr-x   0        0        0      488 2023-12-28 21:20:40.362230 pygpt_net-2.2.2/src/pygpt_net/ui/widget/image/__init__.py
+-rwxr-xr-x   0        0        0     3797 2024-03-26 17:12:51.298308 pygpt_net-2.2.2/src/pygpt_net/ui/widget/image/display.py
+-rwxr-xr-x   0        0        0      488 2023-12-28 21:20:40.362230 pygpt_net-2.2.2/src/pygpt_net/ui/widget/lists/__init__.py
+-rwxr-xr-x   0        0        0     2682 2024-01-29 13:41:53.379769 pygpt_net-2.2.2/src/pygpt_net/ui/widget/lists/assistant.py
+-rw-r--r--   0        0        0     1956 2024-04-26 21:55:50.679597 pygpt_net-2.2.2/src/pygpt_net/ui/widget/lists/assistant_store.py
+-rwxr-xr-x   0        0        0     7055 2024-04-14 20:50:29.556142 pygpt_net-2.2.2/src/pygpt_net/ui/widget/lists/attachment.py
+-rwxr-xr-x   0        0        0     2446 2024-04-10 01:07:30.188635 pygpt_net-2.2.2/src/pygpt_net/ui/widget/lists/base.py
+-rwxr-xr-x   0        0        0    17502 2024-04-17 01:35:30.430055 pygpt_net-2.2.2/src/pygpt_net/ui/widget/lists/context.py
+-rw-r--r--   0        0        0     5861 2024-04-17 01:35:30.430055 pygpt_net-2.2.2/src/pygpt_net/ui/widget/lists/db.py
+-rw-r--r--   0        0        0     3658 2024-03-07 01:04:26.449956 pygpt_net-2.2.2/src/pygpt_net/ui/widget/lists/debug.py
+-rw-r--r--   0        0        0     4818 2024-04-17 01:35:30.430055 pygpt_net-2.2.2/src/pygpt_net/ui/widget/lists/index.py
+-rw-r--r--   0        0        0     6794 2024-04-27 14:05:11.727541 pygpt_net-2.2.2/src/pygpt_net/ui/widget/lists/index_combo.py
+-rwxr-xr-x   0        0        0     1080 2023-12-28 21:20:40.362230 pygpt_net-2.2.2/src/pygpt_net/ui/widget/lists/mode.py
+-rwxr-xr-x   0        0        0     1912 2024-01-29 13:41:53.379769 pygpt_net-2.2.2/src/pygpt_net/ui/widget/lists/model.py
+-rw-r--r--   0        0        0     1919 2024-01-29 13:41:53.379769 pygpt_net-2.2.2/src/pygpt_net/ui/widget/lists/model_editor.py
+-rwxr-xr-x   0        0        0     1028 2024-01-12 09:25:47.589375 pygpt_net-2.2.2/src/pygpt_net/ui/widget/lists/plugin.py
+-rwxr-xr-x   0        0        0     4071 2024-02-01 01:48:09.378583 pygpt_net-2.2.2/src/pygpt_net/ui/widget/lists/preset.py
+-rw-r--r--   0        0        0     3899 2024-03-07 01:04:26.449956 pygpt_net-2.2.2/src/pygpt_net/ui/widget/lists/preset_plugins.py
+-rw-r--r--   0        0        0     4432 2024-04-10 01:07:30.192635 pygpt_net-2.2.2/src/pygpt_net/ui/widget/lists/profile.py
+-rw-r--r--   0        0        0     1052 2024-01-12 09:25:47.589375 pygpt_net-2.2.2/src/pygpt_net/ui/widget/lists/settings.py
+-rwxr-xr-x   0        0        0     4382 2024-04-26 21:55:50.679597 pygpt_net-2.2.2/src/pygpt_net/ui/widget/lists/uploaded.py
+-rwxr-xr-x   0        0        0      488 2023-12-28 21:20:40.362230 pygpt_net-2.2.2/src/pygpt_net/ui/widget/option/__init__.py
+-rwxr-xr-x   0        0        0     2068 2024-01-19 21:21:41.774598 pygpt_net-2.2.2/src/pygpt_net/ui/widget/option/checkbox.py
+-rw-r--r--   0        0        0     5503 2024-03-12 06:49:17.172787 pygpt_net-2.2.2/src/pygpt_net/ui/widget/option/cmd.py
+-rw-r--r--   0        0        0     3592 2024-04-27 10:44:46.049374 pygpt_net-2.2.2/src/pygpt_net/ui/widget/option/combo.py
+-rwxr-xr-x   0        0        0    12672 2024-03-11 03:15:21.879593 pygpt_net-2.2.2/src/pygpt_net/ui/widget/option/dictionary.py
+-rwxr-xr-x   0        0        0     9304 2024-04-26 21:55:50.679597 pygpt_net-2.2.2/src/pygpt_net/ui/widget/option/input.py
+-rw-r--r--   0        0        0     2601 2024-04-22 22:35:26.800429 pygpt_net-2.2.2/src/pygpt_net/ui/widget/option/prompt.py
+-rwxr-xr-x   0        0        0     3569 2024-01-08 20:36:28.058493 pygpt_net-2.2.2/src/pygpt_net/ui/widget/option/slider.py
+-rwxr-xr-x   0        0        0     2684 2024-04-26 21:55:50.679597 pygpt_net-2.2.2/src/pygpt_net/ui/widget/option/textarea.py
+-rw-r--r--   0        0        0     1668 2024-01-29 13:41:53.379769 pygpt_net-2.2.2/src/pygpt_net/ui/widget/tabs/Input.py
+-rw-r--r--   0        0        0      488 2023-12-30 09:04:29.205425 pygpt_net-2.2.2/src/pygpt_net/ui/widget/tabs/__init__.py
+-rw-r--r--   0        0        0     2814 2024-04-10 01:07:30.192635 pygpt_net-2.2.2/src/pygpt_net/ui/widget/tabs/output.py
+-rwxr-xr-x   0        0        0      488 2023-12-28 21:20:40.366230 pygpt_net-2.2.2/src/pygpt_net/ui/widget/textarea/__init__.py
+-rw-r--r--   0        0        0     5098 2024-04-21 01:33:54.247764 pygpt_net-2.2.2/src/pygpt_net/ui/widget/textarea/calendar_note.py
+-rw-r--r--   0        0        0     1358 2024-01-28 19:32:28.495073 pygpt_net-2.2.2/src/pygpt_net/ui/widget/textarea/create.py
+-rw-r--r--   0        0        0     5450 2024-04-21 01:33:54.247764 pygpt_net-2.2.2/src/pygpt_net/ui/widget/textarea/editor.py
+-rw-r--r--   0        0        0     1543 2024-04-11 03:43:59.058733 pygpt_net-2.2.2/src/pygpt_net/ui/widget/textarea/find.py
+-rwxr-xr-x   0        0        0     6059 2024-04-22 22:35:26.800429 pygpt_net-2.2.2/src/pygpt_net/ui/widget/textarea/input.py
+-rwxr-xr-x   0        0        0     1132 2024-01-27 21:42:30.964980 pygpt_net-2.2.2/src/pygpt_net/ui/widget/textarea/name.py
+-rwxr-xr-x   0        0        0     6583 2024-04-21 01:33:54.247764 pygpt_net-2.2.2/src/pygpt_net/ui/widget/textarea/notepad.py
+-rwxr-xr-x   0        0        0     5086 2024-04-23 23:11:13.260159 pygpt_net-2.2.2/src/pygpt_net/ui/widget/textarea/output.py
+-rwxr-xr-x   0        0        0     1358 2024-01-28 19:32:28.495073 pygpt_net-2.2.2/src/pygpt_net/ui/widget/textarea/rename.py
+-rwxr-xr-x   0        0        0     1833 2024-04-12 10:08:45.275113 pygpt_net-2.2.2/src/pygpt_net/ui/widget/textarea/search_input.py
+-rwxr-xr-x   0        0        0    10060 2024-04-27 14:05:11.727541 pygpt_net-2.2.2/src/pygpt_net/ui/widget/textarea/web.py
+-rwxr-xr-x   0        0        0      488 2023-12-28 21:20:40.366230 pygpt_net-2.2.2/src/pygpt_net/ui/widget/vision/__init__.py
+-rwxr-xr-x   0        0        0     2584 2023-12-28 21:20:40.366230 pygpt_net-2.2.2/src/pygpt_net/ui/widget/vision/camera.py
+-rwxr-xr-x   0        0        0     5470 2024-04-26 21:55:50.679597 pygpt_net-2.2.2/src/pygpt_net/utils.py
+-rw-r--r--   0        0        0   135709 1970-01-01 00:00:00.000000 pygpt_net-2.2.2/PKG-INFO
```

### Comparing `pygpt_net-2.2.1/CHANGELOG.md` & `pygpt_net-2.2.2/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,17 @@
 # CHANGELOG
 
+# 2.2.2 (2024-04-29)
+
+- Added 'Application environment' option to Config -> General for setting up custom env vars on app load.
+- Added chunk render/parse throttling to prevent high CPU load on huge text chunks.
+- Optimized and improved Code interpreter output rendering in stream mode in Assistants.
+- Improved run stopping in Assistants.
+- Fixed syntax theme and 'Edit' icon restore on profile switch.
+
 # 2.2.1 (2024-04-28)
 
 - Improved data reload on profile switch.
 
 # 2.2.0 (2024-04-28)
 
 - Improved code interpreter stream handling in Assistant mode.
```

### Comparing `pygpt_net-2.2.1/LICENSE` & `pygpt_net-2.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/README.md` & `pygpt_net-2.2.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # PyGPT - Desktop AI Assistant
 
 [![pygpt](https://snapcraft.io/pygpt/badge.svg)](https://snapcraft.io/pygpt)
 
-Release: **2.2.1** | build: **2024.04.28** | Python: **>=3.10, <3.12**
+Release: **2.2.2** | build: **2024.04.29** | Python: **>=3.10, <3.12**
 
 Official website: https://pygpt.net | Documentation: https://pygpt.readthedocs.io
 
 Snap Store: https://snapcraft.io/pygpt | PyPi: https://pypi.org/project/pygpt-net
 
 Compiled version for Linux (`tar.gz`) and Windows 10/11 (`msi`) 64-bit: https://pygpt.net/#download
 
@@ -2667,14 +2667,16 @@
 
 - `Minimize to tray on exit`: Minimize to tray icon on exit. Tray icon enabled is required for this option to work. Default: False.
 
 - `Render engine`: chat output render engine: `WebEngine / Chromium` - for full HTML/CSS and `Legacy (markdown)` for legacy, simple markdown CSS output. Default: WebEngine / Chromium.
 
 - `OpenGL hardware acceleration`: enables hardware acceleration in `WebEngine / Chromium` renderer.  Default: False.
 
+- `Application environment (os.environ)`: Additional environment vars to set on application start.
+
 **Layout**
 
 - `Zoom`: Adjusts the zoom in chat window (web render view). `WebEngine / Chromium` render mode only.
 
 - `Code syntax highlight`: Syntax highlight theme in code blocks. `WebEngine / Chromium` render mode only.
 
 - `Font Size (chat window)`: Adjusts the font size in the chat window (plain-text) and notepads.
@@ -3052,14 +3054,22 @@
 
 ---
 
 # CHANGELOG
 
 ## Recent changes:
 
+**2.2.2 (2024-04-29)**
+
+- Added 'Application environment' option to Config -> General for setting up custom env vars on app load.
+- Added chunk render/parse throttling to prevent high CPU load on huge text chunks.
+- Optimized and improved Code interpreter output rendering in stream mode in Assistants.
+- Improved run stopping in Assistants.
+- Fixed syntax theme and 'Edit' icon restore on profile switch.
+
 **2.2.1 (2024-04-28)**
 
 - Improved data reload on profile switch.
 
 **2.2.0 (2024-04-28)**
 
 - Improved code interpreter stream handling in Assistant mode.
```

### Comparing `pygpt_net-2.2.1/icon.png` & `pygpt_net-2.2.2/icon.png`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/pyproject.toml` & `pygpt_net-2.2.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pygpt-net"
-version = "2.2.1"
+version = "2.2.2"
 description = "Desktop AI Assistant powered by GPT-4, GPT-4V, GPT-3.5, DALL-E 3, Langchain LLMs, Llama-index, Whisper with chatbot, assistant, text completion, vision and image generation, internet access, chat with files, commands and code execution, file upload and download and more"
 authors = ["Marcin Szczyglinski <info@pygpt.net>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/szczyglis-dev/py-gpt"
 repository = "https://github.com/szczyglis-dev/py-gpt"
 documentation = "https://pygpt.readthedocs.io/"
```

### Comparing `pygpt_net-2.2.1/src/pygpt_net/CHANGELOG.txt` & `pygpt_net-2.2.2/src/pygpt_net/CHANGELOG.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,15 @@
+2.2.2 (2024-04-29)
+
+- Added 'Application environment' option to Config -> General for setting up custom env vars on app load.
+- Added chunk render/parse throttling to prevent high CPU load on huge text chunks.
+- Optimized and improved Code interpreter output rendering in stream mode in Assistants.
+- Improved run stopping in Assistants.
+- Fixed syntax theme and 'Edit' icon restore on profile switch.
+
 2.2.1 (2024-04-28)
 
 - Improved data reload on profile switch.
 
 2.2.0 (2024-04-28)
 
 - Improved code interpreter stream handling in Assistant mode.
```

### Comparing `pygpt_net-2.2.1/src/pygpt_net/LICENSE` & `pygpt_net-2.2.2/src/pygpt_net/LICENSE`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/__init__.py` & `pygpt_net-2.2.2/src/pygpt_net/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,23 +2,23 @@
 # -*- coding: utf-8 -*-
 # ================================================== #
 # This file is a part of PYGPT package               #
 # Website: https://pygpt.net                         #
 # GitHub:  https://github.com/szczyglis-dev/py-gpt   #
 # MIT License                                        #
 # Created By  : Marcin Szczygliński                  #
-# Updated Date: 2024.04.28 10:00:00                  #
+# Updated Date: 2024.04.29 07:00:00                  #
 # ================================================== #
 
 __author__ = "Marcin Szczygliński"
 __copyright__ = "Copyright 2024, Marcin Szczygliński"
 __credits__ = ["Marcin Szczygliński"]
 __license__ = "MIT"
-__version__ = "2.2.1"
-__build__ = "2024.04.28"
+__version__ = "2.2.2"
+__build__ = "2024.04.29"
 __maintainer__ = "Marcin Szczygliński"
 __github__ = "https://github.com/szczyglis-dev/py-gpt"
 __website__ = "https://pygpt.net"
 __pypi__ = "https://pypi.org/project/pygpt-net"
 __snap__ = "https://snapcraft.io/pygpt"
 __donate__ = "https://pygpt.net/#donate"
 __documentation__ = "https://pygpt.readthedocs.io"
```

### Comparing `pygpt_net-2.2.1/src/pygpt_net/app.py` & `pygpt_net-2.2.2/src/pygpt_net/app.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/config.py` & `pygpt_net-2.2.2/src/pygpt_net/config.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # -*- coding: utf-8 -*-
 # ================================================== #
 # This file is a part of PYGPT package               #
 # Website: https://pygpt.net                         #
 # GitHub:  https://github.com/szczyglis-dev/py-gpt   #
 # MIT License                                        #
 # Created By  : Marcin Szczygliński                  #
-# Updated Date: 2024.04.11 02:00:00                  #
+# Updated Date: 2024.04.29 07:00:00                  #
 # ================================================== #
 
 import copy
 import datetime
 import os
 import re
 
@@ -502,14 +502,31 @@
         :return: dict with replaced keys
         """
         if key_from in data:
             data[key_to] = copy.deepcopy(data[key_from])
             del data[key_from]
         return data
 
+    def setup_env(self):
+        """Setup environment vars"""
+        if "app.env" not in self.data or not isinstance(self.data["app.env"], list):
+            return
+        list_loaded = []
+        for item in self.data["app.env"]:
+            if item['name'] is None or item['name'] == "":
+                continue
+            try:
+                value = str(item['value'].format(**self.all()))
+                os.environ[item['name']] = value
+                list_loaded.append(item['name'])
+            except Exception as e:
+                print("Error setting env var: {}".format(e))
+        if list_loaded:
+            print("Loaded environment vars: {}".format(", ".join(list_loaded)))
+
     def save(self, filename: str = "config.json"):
         """
         Save config
 
         :param filename: filename
         """
         self.provider.save(self.data, filename)
```

### Comparing `pygpt_net-2.2.1/src/pygpt_net/container.py` & `pygpt_net-2.2.2/src/pygpt_net/container.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # -*- coding: utf-8 -*-
 # ================================================== #
 # This file is a part of PYGPT package               #
 # Website: https://pygpt.net                         #
 # GitHub:  https://github.com/szczyglis-dev/py-gpt   #
 # MIT License                                        #
 # Created By  : Marcin Szczygliński                  #
-# Updated Date: 2024.02.24 00:00:00                  #
+# Updated Date: 2024.04.29 07:00:00                  #
 # ================================================== #
 
 from pygpt_net.config import Config
 from pygpt_net.core.assistants import Assistants
 from pygpt_net.core.attachments import Attachments
 from pygpt_net.core.audio import Audio
 from pygpt_net.core.bridge import Bridge
@@ -88,7 +88,18 @@
         """Initialize all components"""
         self.config.init(all=True)
         self.platforms.init()
 
     def patch(self):
         """Patch version"""
         self.updater.patch()
+
+    def post_setup(self):
+        """Post setup"""
+        self.config.setup_env()
+
+    def reload(self):
+        """Reload core"""
+        self.db.reload()
+        self.patch()
+        self.debug.update_logger_path()
+        self.config.setup_env()
```

### Comparing `pygpt_net-2.2.1/src/pygpt_net/controller/__init__.py` & `pygpt_net-2.2.2/src/pygpt_net/controller/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # -*- coding: utf-8 -*-
 # ================================================== #
 # This file is a part of PYGPT package               #
 # Website: https://pygpt.net                         #
 # GitHub:  https://github.com/szczyglis-dev/py-gpt   #
 # MIT License                                        #
 # Created By  : Marcin Szczygliński                  #
-# Updated Date: 2024.04.28 07:00:00                  #
+# Updated Date: 2024.04.29 07:00:00                  #
 # ================================================== #
 
 from pygpt_net.controller.agent import Agent
 from pygpt_net.controller.assistant import Assistant
 from pygpt_net.controller.attachment import Attachment
 from pygpt_net.controller.audio import Audio
 from pygpt_net.controller.calendar import Calendar
@@ -72,15 +72,15 @@
         self.settings = Settings(window)
         self.theme = Theme(window)
         self.ui = UI(window)
 
     def setup(self):
         """Setup controller"""
         self.debug.setup()  # prepare log level
-        self.chat.render.setup()  # setup render engine
+        self.chat.init()
 
         # setup layout
         self.layout.setup()
         self.ui.setup()
 
         # setup controllers
         self.lang.setup()
@@ -126,44 +126,28 @@
 
     def init(self):
         """Init base settings"""
         self.settings.load()
 
     def reload(self):
         """Reload components"""
-        self.window.core.db.close()  # close current database
-        self.window.core.db.init(force=True)  # re-init database with new path
-        self.window.core.patch()
-        self.window.core.ctx.reset()
-        self.window.core.notepad.locked = True
-        self.window.core.notepad.reset()
-        self.presets.locked = True
-        self.settings.setup()
-        self.window.core.plugins.reload_all()  # reload all plugins
-        self.window.core.presets.load()
-        self.window.core.debug.update_logger_path()
-        self.window.ui.dialogs.app_log.update()
-        self.ctx.setup()
-        self.ctx.update()
-        self.ctx.refresh()
-        self.assistant.setup()
-        self.attachment.setup()
-        self.presets.refresh()
-        self.idx.setup()
-        self.calendar.setup()
-        self.plugins.setup()
-        self.plugins.settings.setup()
-        self.plugins.update()
-        self.painter.setup()
-        self.notepad.update_tabs()
-        self.assistant.store.reset()
-        self.window.core.notepad.locked = False
-        self.files.update_explorer(reload=True)
-        self.lang.reload_config()
-        self.lang.setup()
-        self.theme.setup()
-        self.debug.toggle_menu()
-        self.debug.update()
-        self.chat.common.setup()
+        self.window.core.reload()  # db, config, patch, etc.
+        self.ctx.reload()
+        self.settings.reload()
+        self.assistant.reload()
+        self.attachment.reload()
+        self.presets.reload()
+        self.idx.reload()
+        self.calendar.reload()
+        self.plugins.reload()
+        self.painter.reload()
+        self.notepad.reload()
+        self.files.reload()
+        self.lang.reload()
+        self.theme.reload_all()
+        self.debug.reload()
+        self.chat.reload()
         self.window.tools.on_reload()
-        self.presets.locked = False
-        self.ctx.new_if_empty()  # create new empty context if empty list
+        # self.layout.reload()
+
+        # post-reload
+        self.ctx.reload_after()
```

### Comparing `pygpt_net-2.2.1/src/pygpt_net/controller/agent/__init__.py` & `pygpt_net-2.2.2/src/pygpt_net/controller/agent/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/controller/agent/flow.py` & `pygpt_net-2.2.2/src/pygpt_net/controller/agent/flow.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/controller/assistant/__init__.py` & `pygpt_net-2.2.2/src/pygpt_net/tools/text_editor/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,254 +2,266 @@
 # -*- coding: utf-8 -*-
 # ================================================== #
 # This file is a part of PYGPT package               #
 # Website: https://pygpt.net                         #
 # GitHub:  https://github.com/szczyglis-dev/py-gpt   #
 # MIT License                                        #
 # Created By  : Marcin Szczygliński                  #
-# Updated Date: 2024.04.27 10:00:00                  #
+# Updated Date: 2024.04.14 18:00:00                  #
 # ================================================== #
 
-import webbrowser
+import hashlib
+import os
 
-from pygpt_net.item.assistant import AssistantItem
-
-from .batch import Batch
-from .editor import Editor
-from .files import Files
-from .store import VectorStore
-from .threads import Threads
+from PySide6.QtGui import QAction, QIcon
+from PySide6.QtWidgets import QFileDialog
 
+from pygpt_net.tools.base import BaseTool
+from pygpt_net.tools.text_editor.ui.dialogs import DialogSpawner
 from pygpt_net.utils import trans
 
 
-class Assistant:
-    def __init__(self, window=None):
+class TextEditor(BaseTool):
+    def __init__(self, *args, **kwargs):
         """
-        Assistant controller
+        Text editor
 
         :param window: Window instance
         """
-        self.window = window
-        self.batch = Batch(window)
-        self.editor = Editor(window)
-        self.files = Files(window)
-        self.threads = Threads(window)
-        self.store = VectorStore(window)
+        super(TextEditor, self).__init__(*args, **kwargs)
+        self.id = "editor"
+        self.width = 800
+        self.height = 500
+        self.instance_id = 0
+        self.spawner = None
 
     def setup(self):
-        """Setup assistants"""
-        self.window.core.assistants.load()
-        self.editor.setup()
-        self.update()
-
-    def update(self, update_list: bool = True):
-        """
-        Update assistants list
-
-        :param update_list: update list
-        """
-        if update_list:
-            self.update_list()
-        self.files.update_list()
-        self.select_current()
-
-    def update_list(self):
-        """Update assistants list"""
-        items = self.window.core.assistants.get_all()
-        self.window.ui.toolbox.assistants.update(items)
-
-    def run_stop(self):
-        """Stop assistant run"""
-        ctx = self.window.core.ctx.last_item
-        if ctx is not None:
-            if ctx.run_id is not None and ctx.thread is not None:
-                status = self.window.core.gpt.assistants.run_stop(ctx)
-                if status == "cancelling":
-                    print("Run has been canceled.")
-
-    def prepare(self):
-        """Prepare assistants"""
-        # create or get current thread, it is required before conversation start
-        if self.window.core.config.get('assistant_thread') is None:
-            try:
-                self.window.ui.status(trans('status.sending'))
-                self.window.core.config.set('assistant_thread', self.threads.create_thread())
-            except Exception as e:
-                self.window.core.debug.log(e)
-                self.window.ui.dialogs.alert(e)
+        """Setup tool"""
+        self.spawner = DialogSpawner(self.window)
 
-    def refresh(self):
-        """Update assistants"""
-        self.select_default()
+    def prepare_id(self, file: str):
+        """
+        Prepare unique id for file
 
-    def select(self, idx: int):
+        :param file: file name
+        :return: unique id
         """
-        Select assistant on the list
+        return 'file_editor_' + hashlib.md5(file.encode('utf-8')).hexdigest()
 
-        :param idx: idx on the list
+    def open_file(self, id: str, auto_close: bool = True, force: bool = False, save: bool = False):
         """
-        # check if change is not locked
-        if self.change_locked():
-            return
+        Open text file dialog
 
-        # mark assistant as selected
-        id = self.window.core.assistants.get_by_idx(idx)
-        self.select_by_id(id)
-
-    def select_by_id(self, id: str):
-        """
-        Select assistant on the list
-
-        :param id: assistant ID
-        """
-        self.window.core.config.set('assistant', id)
-
-        # update attachments list with list of attachments from assistant
-        mode = self.window.core.config.get('mode')
-        assistant = self.window.core.assistants.get_by_id(id)
-        self.window.controller.attachment.update()
-        self.update(False)
-
-        # update model if exists in assistant
-        if assistant is not None:
-            model = assistant.model
-            if model is not None and model != "":
-                if model in self.window.core.models.items:
-                    self.window.core.config.set('model', model)
-                    self.window.core.config.data['current_model'][mode] = model
-                    self.window.controller.model.set(mode, model)
-                    self.window.controller.model.update_list()
-                    self.window.controller.model.select_current()
-            self.window.ui.nodes['preset.prompt'].setPlainText(assistant.instructions)
-            self.refresh()
-
-        self.window.controller.ctx.update_ctx()  # update current ctx info
-
-    def from_global(self):
-        """Update current preset from global prompt"""
-        id = self.window.core.config.get('assistant')
-        if id is not None and id != "":
-            if self.window.core.assistants.has(id):
-                assistant = self.window.core.assistants.get_by_id(id)
-                assistant.instructions = self.window.core.config.get('prompt')
-
-    def select_current(self):
-        """Select assistant by current"""
-        assistant_id = self.window.core.config.get('assistant')
-        items = self.window.core.assistants.get_all()
-        if assistant_id in items:
-            idx = list(items.keys()).index(assistant_id)
-            current = self.window.ui.models['assistants'].index(idx, 0)
-            self.window.ui.nodes['assistants'].setCurrentIndex(current)
-            self.window.core.config.set('prompt', items[assistant_id].instructions)
-            self.window.ui.nodes['preset.prompt'].setPlainText(items[assistant_id].instructions)
-
-    def select_default(self):
-        """Set default assistant"""
-        assistant = self.window.core.config.get('assistant')
-        if assistant is None or assistant == "":
-            mode = self.window.core.config.get('mode')
-            if mode == 'assistant':
-                self.window.core.config.set(
-                    'assistant',
-                    self.window.core.assistants.get_default_assistant(),
-                )
-                self.update()
-
-    def create(self) -> AssistantItem:
-        """
-        Create assistant in API
-
-        :return: AssistantItem
-        """
-        assistant = self.window.core.assistants.create()
-        self.editor.assign_data(assistant)
-        try:
-            return self.window.core.gpt.assistants.create(assistant)
-        except Exception as e:
-            self.window.core.debug.log(e)
-            self.window.ui.dialogs.alert(e)
-
-    def update_data(self, assistant: AssistantItem):
-        """
-        Update assistant
-
-        :param assistant: AssistantItem
-        """
-        self.editor.assign_data(assistant)
-        try:
-            return self.window.core.gpt.assistants.update(assistant)
-        except Exception as e:
-            self.window.core.debug.log(e)
-            self.window.ui.dialogs.alert(e)
-
-    def clear(self, force: bool = False):
+        :param id: editor id
+        :param auto_close: auto close current editor
+        :param force: force open new instance
+        :param save: save current file
         """
-        Clear assistant data
+        if not force and self.window.core.filesystem.editor.is_changed(id) and auto_close:
+            self.window.ui.dialogs.confirm(
+                type='editor.changed.open',
+                id=id,
+                msg=trans("changed.confirm"),
+            )
+            return
+
+        if save:
+            self.save(id)
+
+        path, _ = QFileDialog.getOpenFileName(
+            self.window,
+            trans("action.open"))
+        if path:
+            self.open(path, id, auto_close)
 
-        :param force: force clear data
+    def clear(self, id: str = None, force: bool = False, save: bool = False):
         """
-        id = self.window.core.config.get('assistant')
+        Clear current instance
 
-        if not force:
+        :param id: editor id
+        :param force: force open new instance
+        :param save: save current file
+        """
+        if not force and self.window.core.filesystem.editor.is_changed(id):
             self.window.ui.dialogs.confirm(
-                type='assistant_clear',
-                id='',
-                msg=trans('confirm.assistant.clear'),
+                type='editor.changed.clear',
+                id=id,
+                msg=trans("changed.confirm"),
             )
             return
 
-        if id is not None and id != "":
-            if self.window.core.assistants.has(id):
-                assistant = self.window.core.assistants.get_by_id(id)
-                assistant.reset()
-
-        self.window.ui.status(trans('status.assistant.cleared'))
-        self.update()
-
-    def delete(self, idx: int = None, force: bool = False):
-        """
-        Delete assistant
-
-        :param idx: assistant index (row index)
-        :param force: force delete without confirmation
-        """
-        if idx is not None:
-            id = self.window.core.assistants.get_by_idx(idx)
-            if id is not None and id != "":
-                if self.window.core.assistants.has(id):
-                    # if exists then show confirmation dialog
-                    if not force:
-                        self.window.ui.dialogs.confirm(
-                            type='assistant_delete',
-                            id=idx,
-                            msg=trans('confirm.assistant.delete'),
-                        )
-                        return
-
-                    # clear if this is current assistant
-                    if id == self.window.core.config.get('assistant'):
-                        self.window.core.config.set('assistant', None)
-                        self.window.core.config.set('assistant_thread', None)
-
-                    # delete in API
-                    try:
-                        self.window.core.gpt.assistants.delete(id)
-                    except Exception as e:
-                        self.window.ui.dialogs.alert(e)
-
-                    self.window.core.assistants.delete(id)
-                    self.update()
-                    self.window.ui.status(trans('status.assistant.deleted'))
-
-    def goto_online(self):
-        """Open Assistants page"""
-        webbrowser.open('https://platform.openai.com/assistants')
-
-    def change_locked(self) -> bool:
+        if save:
+            id = self.save(id)
+            self.close(id)
+
+        self.window.core.filesystem.editor.clear(id)
+
+    def new(self):
+        """Open new instance"""
+        self.open()
+
+    def open(
+            self,
+            file: str = None,
+            current_id: str = None,
+            auto_close: bool = True,
+            force: bool = False):
+        """
+        Open/toggle file editor
+
+        :param file: File to load
+        :param current_id: editor id
+        :param auto_close: auto close current editor
+        :param force: force open new instance
         """
-        Check if assistant change is locked
+        # pre-check if file can be opened as text
+        if file:
+            try:
+                with open(file, "r", encoding="utf-8") as f:
+                    f.read()
+            except Exception as e:
+                self.window.ui.dialogs.alert(e)
+                self.window.ui.status("Error opening text file: {}".format(e))
+                return
 
-        :return: True if locked
+            # close current editor if different file
+            id = self.prepare_id(file)
+            if current_id and auto_close:
+                if id != current_id:
+                    self.close(current_id)
+        else:
+            # new instance id
+            id = 'file_tmp_editor_' + str(self.instance_id)
+            self.instance_id += 1
+
+        self.window.ui.dialogs.open_instance(
+            id,
+            width=self.width,
+            height=self.height,
+        )
+
+        # set file
+        if file:
+            title = os.path.basename(file)
+            file_size = self.window.core.filesystem.sizeof_fmt(os.path.getsize(file))
+            title += " - {}".format(file_size)
+            self.window.ui.dialog[id].file = file
+            self.window.core.filesystem.editor.load(id, file)  # load file to editor
+            self.window.ui.dialog[id].setWindowTitle(title)  # set window title
+            self.window.ui.editor[id].setFocus()  # set focus
+            if not force:
+                self.window.ui.status("Loaded file: {}".format(os.path.basename(file)))  # set status
+        else:
+            self.window.core.filesystem.editor.clear(id)  # clear editor if no file
+
+    def close(self, id: str, save: bool = False):
+        """
+        Close file editor
+
+        :param id: editor id
+        :param save: save file before close
+        """
+        if save:
+            id = self.save(id)
+        self.window.ui.dialog[id].accept_close = True
+        self.window.core.filesystem.editor.destroy(id)  # unregister from memory
+        self.window.ui.dialogs.close(id)
+
+    def save(self, id: str) -> str:
+        """
+        Save content to current file
+
+        :param id: editor id
+        :return: new editor id
+        """
+        file = self.window.ui.dialog[id].file
+        if file:
+            self.window.core.filesystem.editor.save(id)
+        else:
+            id = self.save_as_file(id)
+        return id
+
+    def restore(self, id: str, force: bool = False, save: bool = False):
+        """
+        Restore file content
+
+        :param id: editor id
+        :param force: force restore
+        :param save: save file before restore
         """
-        return self.window.controller.chat.input.generating
+        if not force and self.window.core.filesystem.editor.is_changed(id):
+            self.window.ui.dialogs.confirm(
+                type='editor.changed.restore',
+                id=id,
+                msg=trans("changed.confirm"),
+            )
+            return
+
+        if save:
+            self.save(id)
+
+        file = self.window.ui.dialog[id].file
+        if file:
+            self.window.core.filesystem.editor.restore(id)
+        else:
+            self.window.ui.dialogs.alert("No file to restore")
+
+    def save_as_file(self, id: str) -> str:
+        """
+        Save content to file
+
+        :param id: editor id
+        :return: new editor id
+        """
+        file_name = ""
+        current = self.window.ui.dialog[id].file
+        if current:
+            file_name = os.path.basename(current)
+        path, _ = QFileDialog.getSaveFileName(
+            self.window,
+            trans("action.save_as"),
+            file_name,
+        )
+        if path:
+            self.window.core.filesystem.editor.save(id, path)
+        return id
+
+    def setup_menu(self) -> dict:
+        """
+        Setup main menu
+
+        :return dict with menu actions
+        """
+        actions = {}
+        actions["text.editor"] = QAction(
+            QIcon(":/icons/edit.svg"),
+            trans("menu.tools.text.editor"),
+            self.window,
+            checkable=False,
+        )
+        actions["text.editor"].triggered.connect(
+            lambda: self.open()
+        )
+        return actions
+
+    def get_instance(self, type_id: str, dialog_id: str = None):
+        """
+        Spawn and return dialog instance
+
+        :param type_id: dialog instance type ID
+        :param dialog_id: dialog instance ID
+        :return dialog instance
+        """
+        if type_id == "text_editor":
+            return self.spawner.setup(dialog_id)
+
+    def get_lang_mappings(self) -> dict:
+        """
+        Get language mappings
+
+        :return: dict with language mappings
+        """
+        return {
+            'menu.text': {
+                'tools.text.editor': 'menu.tools.text.editor',
+            }
+        }
```

### Comparing `pygpt_net-2.2.1/src/pygpt_net/controller/assistant/batch.py` & `pygpt_net-2.2.2/src/pygpt_net/controller/assistant/batch.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/controller/assistant/editor.py` & `pygpt_net-2.2.2/src/pygpt_net/controller/assistant/editor.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/controller/assistant/files.py` & `pygpt_net-2.2.2/src/pygpt_net/controller/assistant/files.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/controller/assistant/store.py` & `pygpt_net-2.2.2/src/pygpt_net/controller/assistant/store.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/controller/assistant/threads.py` & `pygpt_net-2.2.2/src/pygpt_net/controller/assistant/threads.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # -*- coding: utf-8 -*-
 # ================================================== #
 # This file is a part of PYGPT package               #
 # Website: https://pygpt.net                         #
 # GitHub:  https://github.com/szczyglis-dev/py-gpt   #
 # MIT License                                        #
 # Created By  : Marcin Szczygliński                  #
-# Updated Date: 2024.04.28 07:00:00                  #
+# Updated Date: 2024.04.29 07:00:00                  #
 # ================================================== #
 
 import json
 import time
 
 from PySide6.QtCore import QObject, Signal, Slot, QRunnable
 
@@ -350,14 +350,24 @@
         :param ctx: CtxItem
         """
         self.stop = False
         self.window.controller.chat.common.unlock_input()
         self.window.statusChanged.emit(trans('assistant.run.failed'))
         self.window.stateChanged.emit(self.window.STATE_ERROR)
 
+    def handle_run_step_created(self, ctx: CtxItem, stream: bool = False):
+        """
+        Handle run step created (stream and not stream)
+
+        :param ctx: CtxItem
+        :param stream: True if stream
+        """
+        self.window.stateChanged.emit(self.window.STATE_BUSY)
+        self.window.controller.chat.common.lock_input()  # lock input, show stop button
+
     @Slot(object, object)
     def handle_status(self, run, ctx: CtxItem):
         """
         Handle status (not stream ONLY)
 
         :param run: Run
         :param ctx: CtxItem
```

### Comparing `pygpt_net-2.2.1/src/pygpt_net/controller/attachment.py` & `pygpt_net-2.2.2/src/pygpt_net/controller/attachment.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # -*- coding: utf-8 -*-
 # ================================================== #
 # This file is a part of PYGPT package               #
 # Website: https://pygpt.net                         #
 # GitHub:  https://github.com/szczyglis-dev/py-gpt   #
 # MIT License                                        #
 # Created By  : Marcin Szczygliński                  #
-# Updated Date: 2024.04.26 23:00:00                  #
+# Updated Date: 2024.04.29 07:00:00                  #
 # ================================================== #
 
 import os
 from datetime import datetime
 
 from PySide6.QtGui import QImage
 from PySide6.QtWidgets import QFileDialog, QApplication
@@ -486,7 +486,11 @@
                         return True
         elif source.hasText():
             text = source.text()
             if os.path.exists(text):
                 return True
         return False
 
+    def reload(self):
+        """Reload attachments"""
+        self.setup()
+
```

### Comparing `pygpt_net-2.2.1/src/pygpt_net/controller/audio/__init__.py` & `pygpt_net-2.2.2/src/pygpt_net/controller/audio/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/controller/calendar/__init__.py` & `pygpt_net-2.2.2/src/pygpt_net/controller/calendar/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # -*- coding: utf-8 -*-
 # ================================================== #
 # This file is a part of PYGPT package               #
 # Website: https://pygpt.net                         #
 # GitHub:  https://github.com/szczyglis-dev/py-gpt   #
 # MIT License                                        #
 # Created By  : Marcin Szczygliński                  #
-# Updated Date: 2024.03.07 01:00:00                  #
+# Updated Date: 2024.04.29 07:00:00                  #
 # ================================================== #
 
 from .note import Note
 
 
 class Calendar:
     def __init__(self, window=None):
@@ -113,7 +113,11 @@
         """
         Check if calendar tab is active
 
         :return: True if calendar tab is active
         """
         return self.window.ui.tabs['output'].currentIndex() == self.window.controller.ui.tab_idx['calendar']
 
+    def reload(self):
+        """Reload calendar"""
+        self.setup()
+
```

### Comparing `pygpt_net-2.2.1/src/pygpt_net/controller/calendar/note.py` & `pygpt_net-2.2.2/src/pygpt_net/controller/calendar/note.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/controller/camera.py` & `pygpt_net-2.2.2/src/pygpt_net/controller/camera.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/controller/chat/__init__.py` & `pygpt_net-2.2.2/src/pygpt_net/controller/chat/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # -*- coding: utf-8 -*-
 # ================================================== #
 # This file is a part of PYGPT package               #
 # Website: https://pygpt.net                         #
 # GitHub:  https://github.com/szczyglis-dev/py-gpt   #
 # MIT License                                        #
 # Created By  : Marcin Szczygliński                  #
-# Updated Date: 2024.01.13 15:00:00                  #
+# Updated Date: 2024.04.29 07:00:00                  #
 # ================================================== #
 
 from pygpt_net.controller.chat.common import Common
 from pygpt_net.controller.chat.files import Files
 from pygpt_net.controller.chat.image import Image
 from pygpt_net.controller.chat.input import Input
 from pygpt_net.controller.chat.output import Output
@@ -32,10 +32,19 @@
         self.image = Image(window)
         self.input = Input(window)
         self.output = Output(window)
         self.render = Render(window)
         self.text = Text(window)
         self.vision = Vision(window)
 
+    def init(self):
+        """Init"""
+        self.render.setup()  # setup render engine
+
     def setup(self):
         """Setup"""
         self.common.setup()
+
+    def reload(self):
+        """Reload"""
+        self.common.setup()
+        self.render.reload()
```

### Comparing `pygpt_net-2.2.1/src/pygpt_net/controller/chat/common.py` & `pygpt_net-2.2.2/src/pygpt_net/controller/chat/common.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # -*- coding: utf-8 -*-
 # ================================================== #
 # This file is a part of PYGPT package               #
 # Website: https://pygpt.net                         #
 # GitHub:  https://github.com/szczyglis-dev/py-gpt   #
 # MIT License                                        #
 # Created By  : Marcin Szczygliński                  #
-# Updated Date: 2024.04.24 01:00:00                  #
+# Updated Date: 2024.04.29 07:00:00                  #
 # ================================================== #
 
 import os
 
 from PySide6.QtGui import QTextCursor
 from PySide6.QtWidgets import QFileDialog
 
@@ -80,15 +80,18 @@
             self.window.ui.nodes['output_plain'].setVisible(False)
 
         self.window.controller.chat.render.switch(self.initialized)  # switch renderer if needed
 
         # edit icons
         if self.window.core.config.has('ctx.edit_icons'):
             self.window.ui.nodes['output.edit'].setChecked(self.window.core.config.get('ctx.edit_icons'))
-            self.window.controller.chat.render.on_enable_edit(self.initialized)
+            if self.window.core.config.get('ctx.edit_icons'):
+                self.window.controller.chat.render.on_enable_edit(self.initialized)
+            else:
+                self.window.controller.chat.render.on_disable_edit(self.initialized)
 
         # images generation
         if self.window.core.config.get('img_raw'):
             self.window.ui.config['global']['img_raw'].setChecked(True)
         else:
             self.window.ui.config['global']['img_raw'].setChecked(False)
```

### Comparing `pygpt_net-2.2.1/src/pygpt_net/controller/chat/files.py` & `pygpt_net-2.2.2/src/pygpt_net/controller/chat/files.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/controller/chat/image.py` & `pygpt_net-2.2.2/src/pygpt_net/controller/chat/image.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/controller/chat/input.py` & `pygpt_net-2.2.2/src/pygpt_net/controller/chat/input.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/controller/chat/output.py` & `pygpt_net-2.2.2/src/pygpt_net/controller/chat/output.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/controller/chat/render.py` & `pygpt_net-2.2.2/src/pygpt_net/controller/chat/render.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/controller/chat/text.py` & `pygpt_net-2.2.2/src/pygpt_net/controller/chat/text.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/controller/chat/vision.py` & `pygpt_net-2.2.2/src/pygpt_net/controller/chat/vision.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/controller/command.py` & `pygpt_net-2.2.2/src/pygpt_net/controller/command.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/controller/config/__init__.py` & `pygpt_net-2.2.2/src/pygpt_net/controller/config/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/controller/config/field/checkbox.py` & `pygpt_net-2.2.2/src/pygpt_net/controller/config/field/checkbox.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/controller/config/field/cmd.py` & `pygpt_net-2.2.2/src/pygpt_net/controller/config/field/cmd.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/controller/config/field/combo.py` & `pygpt_net-2.2.2/src/pygpt_net/controller/config/field/combo.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/controller/config/field/dictionary.py` & `pygpt_net-2.2.2/src/pygpt_net/controller/config/field/dictionary.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/controller/config/field/input.py` & `pygpt_net-2.2.2/src/pygpt_net/controller/config/field/input.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/controller/config/field/slider.py` & `pygpt_net-2.2.2/src/pygpt_net/controller/config/field/slider.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/controller/config/field/textarea.py` & `pygpt_net-2.2.2/src/pygpt_net/controller/config/field/textarea.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/controller/config/placeholder.py` & `pygpt_net-2.2.2/src/pygpt_net/controller/config/placeholder.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/controller/ctx/__init__.py` & `pygpt_net-2.2.2/src/pygpt_net/controller/ctx/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # -*- coding: utf-8 -*-
 # ================================================== #
 # This file is a part of PYGPT package               #
 # Website: https://pygpt.net                         #
 # GitHub:  https://github.com/szczyglis-dev/py-gpt   #
 # MIT License                                        #
 # Created By  : Marcin Szczygliński                  #
-# Updated Date: 2024.04.28 07:00:00                  #
+# Updated Date: 2024.04.29 07:00:00                  #
 # ================================================== #
 
 from PySide6.QtCore import QModelIndex
 
 from pygpt_net.core.dispatcher import Event
 from pygpt_net.item.ctx import CtxItem
 
@@ -83,15 +83,15 @@
 
         :param reload: reload ctx list items
         :param all: update all
         :param select: select current ctx
         """
         # reload ctx list items
         if reload:
-            self.reload(True)
+            self.update_list(True)
 
         # select current ctx on list
         if select:
             self.select_by_current()
 
         # update all
         if all:
@@ -234,15 +234,15 @@
         Add ctx item (CtxItem object)
 
         :param ctx: CtxItem
         """
         self.window.core.ctx.add(ctx)
         self.update()
 
-    def reload(self, reload: bool = False):
+    def update_list(self, reload: bool = False):
         """
         Reload current ctx list
 
         :param reload: reload ctx list items
         """
         self.window.ui.contexts.ctx_list.update(
             'ctx.list',
@@ -914,7 +914,18 @@
             return
         group = self.window.core.ctx.get_group_by_id(id)
         if group is not None:
             self.window.core.ctx.remove_group(group, all=True)
             if self.group_id == id:
                 self.group_id = None
             self.update()
+
+    def reload(self):
+        """Reload ctx"""
+        self.window.core.ctx.reset()
+        self.setup()
+        self.update()
+        self.refresh()
+
+    def reload_after(self):
+        """After reload"""
+        self.new_if_empty()
```

### Comparing `pygpt_net-2.2.1/src/pygpt_net/controller/ctx/common.py` & `pygpt_net-2.2.2/src/pygpt_net/controller/ctx/common.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/controller/ctx/extra.py` & `pygpt_net-2.2.2/src/pygpt_net/controller/ctx/extra.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/controller/ctx/summarizer.py` & `pygpt_net-2.2.2/src/pygpt_net/controller/ctx/summarizer.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/controller/debug/__init__.py` & `pygpt_net-2.2.2/src/pygpt_net/controller/debug/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # -*- coding: utf-8 -*-
 # ================================================== #
 # This file is a part of PYGPT package               #
 # Website: https://pygpt.net                         #
 # GitHub:  https://github.com/szczyglis-dev/py-gpt   #
 # MIT License                                        #
 # Created By  : Marcin Szczygliński                  #
-# Updated Date: 2024.04.26 23:00:00                  #
+# Updated Date: 2024.04.29 07:00:00                  #
 # ================================================== #
 
 from datetime import datetime
 from logging import ERROR, WARNING, INFO, DEBUG
 
 from PySide6.QtCore import Slot
 from PySide6.QtGui import QTextCursor
@@ -229,7 +229,12 @@
             self.window.ui.dialogs.app_log.reload()
             self.is_app_log = True
 
         self.log('debug.' + id + ' toggled')
 
         # update menu
         self.update()
+
+    def reload(self):
+        """Reload debug"""
+        self.toggle_menu()
+        self.update()
```

### Comparing `pygpt_net-2.2.1/src/pygpt_net/controller/dialogs/__init__.py` & `pygpt_net-2.2.2/src/pygpt_net/controller/dialogs/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/controller/dialogs/confirm.py` & `pygpt_net-2.2.2/src/pygpt_net/controller/dialogs/confirm.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/controller/dialogs/debug.py` & `pygpt_net-2.2.2/src/pygpt_net/controller/dialogs/debug.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/controller/dialogs/info.py` & `pygpt_net-2.2.2/src/pygpt_net/controller/dialogs/info.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/controller/files.py` & `pygpt_net-2.2.2/src/pygpt_net/controller/files.py`

 * *Files 0% similar despite different names*

```diff
@@ -442,7 +442,11 @@
         :return: stripped path
         """
         work_dir = self.window.core.config.get_user_dir("data")
         path = path.replace(work_dir, "")
         if path.startswith("/") or path.startswith("\\"):
             path = path[1:]
         return path
+
+    def reload(self):
+        """Reload files"""
+        self.update_explorer(reload=True)
```

### Comparing `pygpt_net-2.2.1/src/pygpt_net/controller/finder.py` & `pygpt_net-2.2.2/src/pygpt_net/controller/finder.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/controller/idx/__init__.py` & `pygpt_net-2.2.2/src/pygpt_net/controller/idx/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # -*- coding: utf-8 -*-
 # ================================================== #
 # This file is a part of PYGPT package               #
 # Website: https://pygpt.net                         #
 # GitHub:  https://github.com/szczyglis-dev/py-gpt   #
 # MIT License                                        #
 # Created By  : Marcin Szczygliński                  #
-# Updated Date: 2024.04.27 14:00:00                  #
+# Updated Date: 2024.04.29 07:00:00                  #
 # ================================================== #
 
 import datetime
 
 from pygpt_net.item.ctx import CtxItem
 from pygpt_net.utils import trans
 from .common import Common
@@ -227,7 +227,11 @@
     def change_locked(self) -> bool:
         """
         Check if change is locked
 
         :return: True if locked
         """
         return self.locked
+
+    def reload(self):
+        """Reload indexer"""
+        self.setup()
```

### Comparing `pygpt_net-2.2.1/src/pygpt_net/controller/idx/common.py` & `pygpt_net-2.2.2/src/pygpt_net/controller/idx/common.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/controller/idx/indexer.py` & `pygpt_net-2.2.2/src/pygpt_net/controller/idx/indexer.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/controller/idx/settings.py` & `pygpt_net-2.2.2/src/pygpt_net/controller/idx/settings.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/controller/lang/__init__.py` & `pygpt_net-2.2.2/src/pygpt_net/controller/lang/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # -*- coding: utf-8 -*-
 # ================================================== #
 # This file is a part of PYGPT package               #
 # Website: https://pygpt.net                         #
 # GitHub:  https://github.com/szczyglis-dev/py-gpt   #
 # MIT License                                        #
 # Created By  : Marcin Szczygliński                  #
-# Updated Date: 2024.04.11 02:00:00                  #
+# Updated Date: 2024.04.29 07:00:00                  #
 # ================================================== #
 
 from PySide6.QtGui import QAction
 
 from pygpt_net.utils import trans, trans_reload
 from .custom import Custom
 from .mapping import Mapping
@@ -89,7 +89,12 @@
             self.window.core.debug.log(e)
 
         # reload UI
         self.window.controller.ctx.common.update_label_by_current()
         self.window.controller.ctx.update(True, False)
         self.window.controller.ui.update()  # update all (toolbox, etc.)
         self.window.ui.status('')  # clear status
+
+    def reload(self):
+        """Reload language"""
+        self.reload_config()
+        self.setup()
```

### Comparing `pygpt_net-2.2.1/src/pygpt_net/controller/lang/custom.py` & `pygpt_net-2.2.2/src/pygpt_net/controller/lang/custom.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/controller/lang/mapping.py` & `pygpt_net-2.2.2/src/pygpt_net/controller/lang/mapping.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/controller/lang/plugins.py` & `pygpt_net-2.2.2/src/pygpt_net/controller/lang/plugins.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/controller/lang/settings.py` & `pygpt_net-2.2.2/src/pygpt_net/controller/lang/settings.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/controller/launcher.py` & `pygpt_net-2.2.2/src/pygpt_net/controller/launcher.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/controller/layout.py` & `pygpt_net-2.2.2/src/pygpt_net/controller/layout.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # -*- coding: utf-8 -*-
 # ================================================== #
 # This file is a part of PYGPT package               #
 # Website: https://pygpt.net                         #
 # GitHub:  https://github.com/szczyglis-dev/py-gpt   #
 # MIT License                                        #
 # Created By  : Marcin Szczygliński                  #
-# Updated Date: 2024.04.20 06:00:00                  #
+# Updated Date: 2024.04.29 07:00:00                  #
 # ================================================== #
 
 import os
 
 from PySide6.QtWidgets import QApplication
 from PySide6.QtCore import QRect
 
@@ -278,7 +278,11 @@
                 self.window.core.settings.load_editor(current_file)
 
         # show success message
         self.window.ui.dialogs.alert(trans('dialog.css.restore.confirm.success'))
         self.window.core.debug.info("Reloading theme...")
         self.window.controller.theme.reload(force=True)  # reload theme
         self.window.core.debug.info("Theme reloaded.")
+
+    def reload(self):
+        """Reload layout"""
+        self.post_setup()
```

### Comparing `pygpt_net-2.2.1/src/pygpt_net/controller/mode.py` & `pygpt_net-2.2.2/src/pygpt_net/controller/mode.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # -*- coding: utf-8 -*-
 # ================================================== #
 # This file is a part of PYGPT package               #
 # Website: https://pygpt.net                         #
 # GitHub:  https://github.com/szczyglis-dev/py-gpt   #
 # MIT License                                        #
 # Created By  : Marcin Szczygliński                  #
-# Updated Date: 2024.03.15 15:00:00                  #
+# Updated Date: 2024.04.29 07:00:00                  #
 # ================================================== #
 
 from pygpt_net.core.dispatcher import Event
 from pygpt_net.item.ctx import CtxItem
 from pygpt_net.utils import trans
 
 
@@ -36,14 +36,15 @@
         mode = self.window.core.modes.get_by_idx(idx)
         self.set(mode)
 
         event = Event(Event.MODE_SELECT, {
             'value': mode,
         })
         self.window.core.dispatcher.dispatch(event)
+        self.window.controller.attachment.update()
 
     def set(self, mode: str):
         """
         Set mode
 
         :param mode: mode name
         """
```

### Comparing `pygpt_net-2.2.1/src/pygpt_net/controller/model/__init__.py` & `pygpt_net-2.2.2/src/pygpt_net/controller/model/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/controller/model/editor.py` & `pygpt_net-2.2.2/src/pygpt_net/controller/model/editor.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/controller/notepad.py` & `pygpt_net-2.2.2/src/pygpt_net/controller/notepad.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # -*- coding: utf-8 -*-
 # ================================================== #
 # This file is a part of PYGPT package               #
 # Website: https://pygpt.net                         #
 # GitHub:  https://github.com/szczyglis-dev/py-gpt   #
 # MIT License                                        #
 # Created By  : Marcin Szczygliński                  #
-# Updated Date: 2024.04.10 23:00:00                  #
+# Updated Date: 2024.04.29 07:00:00                  #
 # ================================================== #
 
 from PySide6.QtGui import QIcon, QTextCursor
 
 from pygpt_net.item.notepad import NotepadItem
 from pygpt_net.ui.widget.textarea.notepad import NotepadWidget
 from pygpt_net.utils import trans
@@ -319,7 +319,14 @@
         if self.window.controller.ui.current_tab < self.start_tab_idx:
             self.window.ui.tabs['output'].setCurrentIndex(self.start_tab_idx)
         self.window.activateWindow()  # focus
 
     def update(self):
         """Update notepads UI"""
         pass
+
+    def reload(self):
+        """Reload notepads"""
+        self.window.core.notepad.locked = True
+        self.window.core.notepad.reset()
+        self.update_tabs()
+        self.window.core.notepad.locked = False
```

### Comparing `pygpt_net-2.2.1/src/pygpt_net/controller/painter/__init__.py` & `pygpt_net-2.2.2/src/pygpt_net/controller/painter/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # -*- coding: utf-8 -*-
 # ================================================== #
 # This file is a part of PYGPT package               #
 # Website: https://pygpt.net                         #
 # GitHub:  https://github.com/szczyglis-dev/py-gpt   #
 # MIT License                                        #
 # Created By  : Marcin Szczygliński                  #
-# Updated Date: 2024.04.09 23:00:00                  #
+# Updated Date: 2024.04.29 07:00:00                  #
 # ================================================== #
 
 import os
 
 from .capture import Capture
 from .common import Common
 
@@ -76,7 +76,11 @@
     def is_active(self) -> bool:
         """
         Check if painter is enabled
 
         :return: True if painter is current active tab
         """
         return self.window.controller.ui.current_tab == self.window.controller.ui.tab_idx['draw']
+
+    def reload(self):
+        """Reload painter"""
+        self.setup()
```

### Comparing `pygpt_net-2.2.1/src/pygpt_net/controller/painter/capture.py` & `pygpt_net-2.2.2/src/pygpt_net/controller/painter/capture.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/controller/painter/common.py` & `pygpt_net-2.2.2/src/pygpt_net/controller/painter/common.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/controller/plugins/__init__.py` & `pygpt_net-2.2.2/src/pygpt_net/controller/plugins/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # -*- coding: utf-8 -*-
 # ================================================== #
 # This file is a part of PYGPT package               #
 # Website: https://pygpt.net                         #
 # GitHub:  https://github.com/szczyglis-dev/py-gpt   #
 # MIT License                                        #
 # Created By  : Marcin Szczygliński                  #
-# Updated Date: 2024.03.25 10:00:00                  #
+# Updated Date: 2024.04.29 07:00:00                  #
 # ================================================== #
 
 from PySide6.QtGui import QAction
 
 from pygpt_net.controller.plugins.presets import Presets
 from pygpt_net.controller.plugins.settings import Settings
 from pygpt_net.core.dispatcher import Event
@@ -413,7 +413,14 @@
         # dispatch inline command event
         event = Event(Event.CMD_INLINE, {
             'commands': commands,
         })
         ctx.results = []
         event.ctx = ctx
         self.window.controller.command.dispatch(event)
+
+    def reload(self):
+        """Reload plugins"""
+        self.window.core.plugins.reload_all()  # reload all plugin options
+        self.setup()
+        self.settings.setup()
+        self.update()
```

### Comparing `pygpt_net-2.2.1/src/pygpt_net/controller/plugins/presets.py` & `pygpt_net-2.2.2/src/pygpt_net/controller/plugins/presets.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/controller/plugins/settings.py` & `pygpt_net-2.2.2/src/pygpt_net/controller/plugins/settings.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/controller/presets/__init__.py` & `pygpt_net-2.2.2/src/pygpt_net/controller/presets/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # -*- coding: utf-8 -*-
 # ================================================== #
 # This file is a part of PYGPT package               #
 # Website: https://pygpt.net                         #
 # GitHub:  https://github.com/szczyglis-dev/py-gpt   #
 # MIT License                                        #
 # Created By  : Marcin Szczygliński                  #
-# Updated Date: 2024.04.22 23:00:00                  #
+# Updated Date: 2024.04.29 07:00:00                  #
 # ================================================== #
 
 import re
 
 from PySide6.QtGui import QTextCursor
 
 from pygpt_net.controller.presets.editor import Editor
@@ -414,7 +414,14 @@
         """
         # if self.window.controller.chat.input.generating:
         # return True
         mode = self.window.core.config.get('mode')
         if mode == "assistant":
             return True
         return False
+
+    def reload(self):
+        """Reload presets"""
+        self.locked = True
+        self.window.core.presets.load()
+        self.refresh()
+        self.locked = False
```

### Comparing `pygpt_net-2.2.1/src/pygpt_net/controller/presets/editor.py` & `pygpt_net-2.2.2/src/pygpt_net/controller/presets/editor.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/controller/settings/__init__.py` & `pygpt_net-2.2.2/src/pygpt_net/controller/settings/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # -*- coding: utf-8 -*-
 # ================================================== #
 # This file is a part of PYGPT package               #
 # Website: https://pygpt.net                         #
 # GitHub:  https://github.com/szczyglis-dev/py-gpt   #
 # MIT License                                        #
 # Created By  : Marcin Szczygliński                  #
-# Updated Date: 2024.04.09 23:00:00                  #
+# Updated Date: 2024.04.29 07:00:00                  #
 # ================================================== #
 
 import os
 
 from .editor import Editor
 from .profile import Profile
 from .workdir import Workdir
@@ -227,7 +227,12 @@
             self.window.ui.status('Config directory not exists: {}'.format(self.window.core.config.path))
 
     def welcome_settings(self):
         """Open settings at first launch (if no API key yet)"""
         self.open_section("general")
         self.window.ui.config['config']['api_key'].setFocus()
         self.window.ui.dialogs.close('info.start')
+
+    def reload(self):
+        """Reload settings"""
+        self.setup()
+        self.window.ui.dialogs.app_log.update()
```

### Comparing `pygpt_net-2.2.1/src/pygpt_net/controller/settings/editor.py` & `pygpt_net-2.2.2/src/pygpt_net/controller/settings/editor.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/controller/settings/profile.py` & `pygpt_net-2.2.2/src/pygpt_net/controller/settings/profile.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # -*- coding: utf-8 -*-
 # ================================================== #
 # This file is a part of PYGPT package               #
 # Website: https://pygpt.net                         #
 # GitHub:  https://github.com/szczyglis-dev/py-gpt   #
 # MIT License                                        #
 # Created By  : Marcin Szczygliński                  #
-# Updated Date: 2024.04.19 01:00:00                  #
+# Updated Date: 2024.04.29 07:00:00                  #
 # ================================================== #
 
 import copy
 import os
 from pathlib import Path
 from uuid import uuid4
 
@@ -57,14 +57,15 @@
             self.window.ui.dialogs.alert("Profile not found!")
             return
         self.window.ui.status("Please wait...")
 
         if save_current:
             print("Saving all settings in current profile...")
             self.window.controller.settings.save_all(force=True)  # save all current settings
+            # self.window.controller.layout.save()  # save layout state
         self.window.core.config.profile.set_current(uuid)
 
         # switch to profile workdir
         path = self.window.core.config.profile.get_current_workdir()
         if path and os.path.exists(path):
             self.window.controller.settings.workdir.update(path, force=True)
```

### Comparing `pygpt_net-2.2.1/src/pygpt_net/controller/settings/workdir.py` & `pygpt_net-2.2.2/src/pygpt_net/controller/settings/workdir.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/controller/theme/__init__.py` & `pygpt_net-2.2.2/src/pygpt_net/controller/theme/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # -*- coding: utf-8 -*-
 # ================================================== #
 # This file is a part of PYGPT package               #
 # Website: https://pygpt.net                         #
 # GitHub:  https://github.com/szczyglis-dev/py-gpt   #
 # MIT License                                        #
 # Created By  : Marcin Szczygliński                  #
-# Updated Date: 2024.04.24 02:00:00                  #
+# Updated Date: 2024.04.29 07:00:00                  #
 # ================================================== #
 
 import os
 
 from .common import Common
 from .markdown import Markdown
 from .menu import Menu
@@ -108,14 +108,15 @@
         """
         Toggle syntax highlight
 
         :param name: syntax style name
         :param update_menu: update menu
         """
         self.window.core.config.set("render.code_syntax", name)
+        self.window.core.config.save()
         self.window.controller.chat.render.on_theme_change()
         if update_menu:
             self.menu.update_syntax()
 
     def reload(self, force: bool = True):
         """
         Reload current theme
@@ -166,7 +167,11 @@
         """
         Return CSS style for element (alias)
 
         :param element: type of element
         :return: CSS style for element
         """
         return self.common.get_style(element)
+
+    def reload_all(self):
+        """Reload all"""
+        self.setup()
```

### Comparing `pygpt_net-2.2.1/src/pygpt_net/controller/theme/common.py` & `pygpt_net-2.2.2/src/pygpt_net/controller/theme/common.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/controller/theme/markdown.py` & `pygpt_net-2.2.2/src/pygpt_net/controller/theme/markdown.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/controller/theme/menu.py` & `pygpt_net-2.2.2/src/pygpt_net/controller/theme/menu.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/controller/theme/nodes.py` & `pygpt_net-2.2.2/src/pygpt_net/controller/theme/nodes.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/controller/ui/__init__.py` & `pygpt_net-2.2.2/src/pygpt_net/controller/ui/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/controller/ui/mode.py` & `pygpt_net-2.2.2/src/pygpt_net/controller/ui/mode.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/controller/ui/vision.py` & `pygpt_net-2.2.2/src/pygpt_net/controller/ui/vision.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/core/assistants/__init__.py` & `pygpt_net-2.2.2/src/pygpt_net/core/assistants/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/core/assistants/files.py` & `pygpt_net-2.2.2/src/pygpt_net/core/assistants/files.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/core/assistants/store.py` & `pygpt_net-2.2.2/src/pygpt_net/core/assistants/store.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/core/attachments.py` & `pygpt_net-2.2.2/src/pygpt_net/core/attachments.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/core/audio.py` & `pygpt_net-2.2.2/src/pygpt_net/core/audio.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/core/bridge.py` & `pygpt_net-2.2.2/src/pygpt_net/core/bridge.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/core/calendar/__init__.py` & `pygpt_net-2.2.2/src/pygpt_net/core/calendar/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/core/camera.py` & `pygpt_net-2.2.2/src/pygpt_net/core/camera.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/core/chain/__init__.py` & `pygpt_net-2.2.2/src/pygpt_net/core/chain/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/core/chain/chat.py` & `pygpt_net-2.2.2/src/pygpt_net/core/chain/chat.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/core/chain/completion.py` & `pygpt_net-2.2.2/src/pygpt_net/core/chain/completion.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/core/command.py` & `pygpt_net-2.2.2/src/pygpt_net/core/command.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/core/ctx/__init__.py` & `pygpt_net-2.2.2/src/pygpt_net/core/ctx/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/core/ctx/idx.py` & `pygpt_net-2.2.2/src/pygpt_net/core/ctx/idx.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/core/db/__init__.py` & `pygpt_net-2.2.2/src/pygpt_net/core/db/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # -*- coding: utf-8 -*-
 # ================================================== #
 # This file is a part of PYGPT package               #
 # Website: https://pygpt.net                         #
 # GitHub:  https://github.com/szczyglis-dev/py-gpt   #
 # MIT License                                        #
 # Created By  : Marcin Szczygliński                  #
-# Updated Date: 2024.04.26 23:00:00                  #
+# Updated Date: 2024.04.29 07:00:00                  #
 # ================================================== #
 
 import os
 import shutil
 import time
 
 from sqlalchemy import create_engine, text
@@ -483,7 +483,12 @@
         else:
             stmt = text("""
                 INSERT INTO config (config_key, config_value, created_ts, updated_ts) 
                 VALUES (:key, :value, :created_ts, :updated_ts)
             """).bindparams(key=key, value=value, created_ts=ts, updated_ts=ts)
 
         conn.execute(stmt)
+
+    def reload(self):
+        """Reload database connection"""
+        self.close()  # close current database
+        self.init(force=True)  # re-init database with new path
```

### Comparing `pygpt_net-2.2.1/src/pygpt_net/core/db/viewer.py` & `pygpt_net-2.2.2/src/pygpt_net/core/db/viewer.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/core/debug/__init__.py` & `pygpt_net-2.2.2/src/pygpt_net/core/debug/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/core/debug/agent.py` & `pygpt_net-2.2.2/src/pygpt_net/core/debug/agent.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/core/debug/assistants.py` & `pygpt_net-2.2.2/src/pygpt_net/core/debug/assistants.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/core/debug/attachments.py` & `pygpt_net-2.2.2/src/pygpt_net/core/debug/attachments.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/core/debug/config.py` & `pygpt_net-2.2.2/src/pygpt_net/core/debug/config.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/core/debug/context.py` & `pygpt_net-2.2.2/src/pygpt_net/core/debug/context.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/core/debug/db.py` & `pygpt_net-2.2.2/src/pygpt_net/core/debug/db.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/core/debug/indexes.py` & `pygpt_net-2.2.2/src/pygpt_net/core/debug/indexes.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/core/debug/models.py` & `pygpt_net-2.2.2/src/pygpt_net/core/debug/models.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/core/debug/plugins.py` & `pygpt_net-2.2.2/src/pygpt_net/core/debug/plugins.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/core/debug/presets.py` & `pygpt_net-2.2.2/src/pygpt_net/core/debug/presets.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/core/debug/ui.py` & `pygpt_net-2.2.2/src/pygpt_net/core/debug/ui.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/core/dispatcher.py` & `pygpt_net-2.2.2/src/pygpt_net/core/dispatcher.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/core/filesystem/__init__.py` & `pygpt_net-2.2.2/src/pygpt_net/core/filesystem/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/core/filesystem/actions.py` & `pygpt_net-2.2.2/src/pygpt_net/core/filesystem/actions.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/core/filesystem/editor.py` & `pygpt_net-2.2.2/src/pygpt_net/core/filesystem/editor.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/core/filesystem/types.py` & `pygpt_net-2.2.2/src/pygpt_net/core/filesystem/types.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/core/filesystem/url.py` & `pygpt_net-2.2.2/src/pygpt_net/core/filesystem/url.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/core/history.py` & `pygpt_net-2.2.2/src/pygpt_net/core/history.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/core/idx/__init__.py` & `pygpt_net-2.2.2/src/pygpt_net/core/idx/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/core/idx/chat.py` & `pygpt_net-2.2.2/src/pygpt_net/core/idx/chat.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/core/idx/context.py` & `pygpt_net-2.2.2/src/pygpt_net/core/idx/context.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/core/idx/indexing.py` & `pygpt_net-2.2.2/src/pygpt_net/core/idx/indexing.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/core/idx/llm.py` & `pygpt_net-2.2.2/src/pygpt_net/core/idx/llm.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/core/idx/metadata.py` & `pygpt_net-2.2.2/src/pygpt_net/core/idx/metadata.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/core/idx/types/ctx.py` & `pygpt_net-2.2.2/src/pygpt_net/core/idx/types/ctx.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/core/idx/types/external.py` & `pygpt_net-2.2.2/src/pygpt_net/core/idx/types/external.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/core/idx/types/files.py` & `pygpt_net-2.2.2/src/pygpt_net/core/idx/types/files.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/core/idx/worker.py` & `pygpt_net-2.2.2/src/pygpt_net/core/idx/worker.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/core/image.py` & `pygpt_net-2.2.2/src/pygpt_net/core/image.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/core/info.py` & `pygpt_net-2.2.2/src/pygpt_net/core/info.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/core/installer.py` & `pygpt_net-2.2.2/src/pygpt_net/core/installer.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/core/llm/__init__.py` & `pygpt_net-2.2.2/src/pygpt_net/core/llm/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/core/locale.py` & `pygpt_net-2.2.2/src/pygpt_net/core/locale.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/core/models.py` & `pygpt_net-2.2.2/src/pygpt_net/core/models.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/core/modes.py` & `pygpt_net-2.2.2/src/pygpt_net/core/modes.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/core/notepad.py` & `pygpt_net-2.2.2/src/pygpt_net/core/notepad.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/core/platforms.py` & `pygpt_net-2.2.2/src/pygpt_net/core/platforms.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/core/plugins.py` & `pygpt_net-2.2.2/src/pygpt_net/core/plugins.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/core/presets.py` & `pygpt_net-2.2.2/src/pygpt_net/core/presets.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/core/profile.py` & `pygpt_net-2.2.2/src/pygpt_net/core/profile.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/core/prompt/__init__.py` & `pygpt_net-2.2.2/src/pygpt_net/core/prompt/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/core/prompt/template.py` & `pygpt_net-2.2.2/src/pygpt_net/core/prompt/template.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/core/render/base.py` & `pygpt_net-2.2.2/src/pygpt_net/core/render/base.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/core/render/markdown/parser.py` & `pygpt_net-2.2.2/src/pygpt_net/core/render/markdown/parser.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/core/render/markdown/renderer.py` & `pygpt_net-2.2.2/src/pygpt_net/core/render/markdown/renderer.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/core/render/plain/renderer.py` & `pygpt_net-2.2.2/src/pygpt_net/core/render/plain/renderer.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/core/render/web/parser.py` & `pygpt_net-2.2.2/src/pygpt_net/core/render/web/parser.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/core/render/web/renderer.py` & `pygpt_net-2.2.2/src/pygpt_net/core/render/web/renderer.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,26 +2,28 @@
 # -*- coding: utf-8 -*-
 # ================================================== #
 # This file is a part of PYGPT package               #
 # Website: https://pygpt.net                         #
 # GitHub:  https://github.com/szczyglis-dev/py-gpt   #
 # MIT License                                        #
 # Created By  : Marcin Szczygliński                  #
-# Updated Date: 2024.04.25 03:00:00                  #
+# Updated Date: 2024.04.29 07:00:00                  #
 # ================================================== #
 
 import json
 import os
 import re
 import html
+import time
 from datetime import datetime
 
 from pygments.formatters.html import HtmlFormatter
 
 from pygpt_net.core.render.base import BaseRenderer
+from pygpt_net.core.text.utils import has_unclosed_code_tag
 from pygpt_net.item.ctx import CtxItem
 from pygpt_net.ui.widget.textarea.input import ChatInput
 from pygpt_net.utils import trans
 from .parser import Parser
 
 
 class Renderer(BaseRenderer):
@@ -47,14 +49,17 @@
         self.document = ""
         self.initialized = False
         self.loaded = False  # page loaded
         self.item = None  # current item
         self.use_buffer = False  # use html buffer
         self.name_user = trans("chat.name.user")
         self.name_bot = trans("chat.name.bot")
+        self.last_time_called = 0
+        self.cooldown = 1 / 6  # max chunks to parse per second
+        self.throttling_min_chars = 3000  # min chunk chars to activate cooldown
 
     def init(self):
         """
         Initialize renderer
         """
         if not self.initialized:
             self.flush()
@@ -226,25 +231,37 @@
 
         :param item: context item
         :param text_chunk: text chunk
         :param begin: if it is the beginning of the text
         """
         self.item = item
         if text_chunk is None or text_chunk == "":
+            if begin:
+                self.buffer = ""  # always reset buffer
             return
 
         self.update_names(item)
         raw_chunk = str(text_chunk)
         if begin:
             self.buffer = ""  # reset buffer
             self.is_cmd = False  # reset command flag
             self.clear_chunks_output()
         self.buffer += raw_chunk
+
+        # cooldown (throttling) to prevent high CPU usage on huge text chunks
+        if len(self.buffer) > self.throttling_min_chars:
+            current_time = time.time()
+            if current_time - self.last_time_called <= self.cooldown:
+                return  # wait a moment
+            else:
+                self.last_time_called = current_time
+
+        # parse chunks
         to_append = self.buffer
-        if re.search(r'```(?!.*```)', self.buffer):
+        if has_unclosed_code_tag(self.buffer):
             to_append += "\n```"  # fix for code block without closing ```
         html = self.parser.parse(to_append)
         escaped_chunk = json.dumps(html)
         try:
             self.get_output_node().page().runJavaScript(f"replaceOutput('{self.name_bot}', {escaped_chunk});")
         except Exception as e:
             pass
```

### Comparing `pygpt_net-2.2.1/src/pygpt_net/core/settings.py` & `pygpt_net-2.2.2/src/pygpt_net/core/settings.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/core/text/finder.py` & `pygpt_net-2.2.2/src/pygpt_net/core/text/finder.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/core/text/utils.py` & `pygpt_net-2.2.2/src/pygpt_net/core/text/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,17 +2,19 @@
 # -*- coding: utf-8 -*-
 # ================================================== #
 # This file is a part of PYGPT package               #
 # Website: https://pygpt.net                         #
 # GitHub:  https://github.com/szczyglis-dev/py-gpt   #
 # MIT License                                        #
 # Created By  : Marcin Szczygliński                  #
-# Updated Date: 2024.04.24 01:00:00                  #
+# Updated Date: 2024.04.29 07:00:00                  #
 # ================================================== #
 
+import re
+
 from bs4 import BeautifulSoup
 
 
 def output_html2text(html: str) -> str:
     """
     Convert output HTML to plain text
 
@@ -56,8 +58,19 @@
             tag.decompose()
         # remove action icons
         for tag in soup.find_all('div', class_='action-icons'):
             tag.decompose()
         return str(soup)
     except Exception as e:
         pass
-    return html
+    return html
+
+def has_unclosed_code_tag(text: str) -> bool:
+    """
+    Check if HTML content has unclosed code block
+
+    :param text: HTML content
+    :return: True if unclosed code block found
+    """
+    if re.search(r'```(?!.*```)', text):
+        return True
+    return False
```

### Comparing `pygpt_net-2.2.1/src/pygpt_net/core/text/web_finder.py` & `pygpt_net-2.2.2/src/pygpt_net/core/text/web_finder.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/core/tokens.py` & `pygpt_net-2.2.2/src/pygpt_net/core/tokens.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/core/updater/__init__.py` & `pygpt_net-2.2.2/src/pygpt_net/core/updater/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/core/web.py` & `pygpt_net-2.2.2/src/pygpt_net/core/web.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/core/worker.py` & `pygpt_net-2.2.2/src/pygpt_net/core/worker.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/data/config/config.json` & `pygpt_net-2.2.2/src/pygpt_net/data/config/config.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9983974358974359%*

 * *Differences: {"'__meta__'": "{'version': '2.2.2', 'app.version': '2.2.2', 'updated_at': '2024-04-29T00:00:00'}"}*

```diff
@@ -1,12 +1,12 @@
 {
     "__meta__": {
-        "app.version": "2.2.1",
-        "updated_at": "2024-04-28T00:00:00",
-        "version": "2.2.1"
+        "app.version": "2.2.2",
+        "updated_at": "2024-04-29T00:00:00",
+        "version": "2.2.2"
     },
     "agent.auto_stop": true,
     "agent.goal.notify": true,
     "agent.idx": "base",
     "agent.iterations": 3,
     "agent.mode": "chat",
     "ai_name": "",
```

### Comparing `pygpt_net-2.2.1/src/pygpt_net/data/config/models.json` & `pygpt_net-2.2.2/src/pygpt_net/data/config/models.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.875%*

 * *Differences: {"'__meta__'": "{'version': '2.2.2', 'app.version': '2.2.2', 'updated_at': '2024-04-29T00:00:00'}"}*

```diff
@@ -1,12 +1,12 @@
 {
     "__meta__": {
-        "app.version": "2.2.1",
-        "updated_at": "2024-04-28T00:00:00",
-        "version": "2.2.1"
+        "app.version": "2.2.2",
+        "updated_at": "2024-04-29T00:00:00",
+        "version": "2.2.2"
     },
     "items": {
         "dall-e-2": {
             "ctx": 0,
             "default": false,
             "id": "dall-e-2",
             "langchain": {
```

### Comparing `pygpt_net-2.2.1/src/pygpt_net/data/config/modes.json` & `pygpt_net-2.2.2/src/pygpt_net/data/config/modes.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.875%*

 * *Differences: {"'__meta__'": "{'version': '2.2.2', 'app.version': '2.2.2', 'updated_at': '2024-04-29T00:00:00'}"}*

```diff
@@ -1,12 +1,12 @@
 {
     "__meta__": {
-        "app.version": "2.2.1",
-        "updated_at": "2024-04-28T00:00:00",
-        "version": "2.2.1"
+        "app.version": "2.2.2",
+        "updated_at": "2024-04-29T00:00:00",
+        "version": "2.2.2"
     },
     "items": {
         "agent": {
             "default": false,
             "id": "agent",
             "label": "mode.agent",
             "name": "Agent (autonomous)"
```

### Comparing `pygpt_net-2.2.1/src/pygpt_net/data/config/presets/current.agent.json` & `pygpt_net-2.2.2/src/pygpt_net/data/config/presets/current.agent.json`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/data/config/settings.json` & `pygpt_net-2.2.2/src/pygpt_net/data/config/settings.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9891304347826086%*

 * *Differences: {"'app.env'": "OrderedDict([('section', 'general'), ('type', 'dict'), ('keys', "*

 * *              "OrderedDict([('name', 'text'), ('value', 'text')])), ('label', 'settings.app.env'), "*

 * *              "('description', 'settings.app.env.desc'), ('value', []), ('advanced', True)])"}*

```diff
@@ -66,14 +66,26 @@
         "secret": true,
         "section": "general",
         "slider": false,
         "step": null,
         "type": "text",
         "value": ""
     },
+    "app.env": {
+        "advanced": true,
+        "description": "settings.app.env.desc",
+        "keys": {
+            "name": "text",
+            "value": "text"
+        },
+        "label": "settings.app.env",
+        "section": "general",
+        "type": "dict",
+        "value": []
+    },
     "context_threshold": {
         "advanced": false,
         "description": "settings.context_threshold.desc",
         "label": "settings.context_threshold",
         "max": 1000,
         "min": 1,
         "multiplier": 1,
```

### Comparing `pygpt_net-2.2.1/src/pygpt_net/data/config/settings_section.json` & `pygpt_net-2.2.2/src/pygpt_net/data/config/settings_section.json`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/data/css/fix_windows.css` & `pygpt_net-2.2.2/src/pygpt_net/data/css/fix_windows.css`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/data/css/markdown.css` & `pygpt_net-2.2.2/src/pygpt_net/data/css/markdown.css`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/data/css/markdown.dark.css` & `pygpt_net-2.2.2/src/pygpt_net/data/css/markdown.dark.css`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/data/css/markdown.light.css` & `pygpt_net-2.2.2/src/pygpt_net/data/css/markdown.light.css`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/data/css/style.dark.css` & `pygpt_net-2.2.2/src/pygpt_net/data/css/style.dark.css`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/data/css/style.light.css` & `pygpt_net-2.2.2/src/pygpt_net/data/css/style.light.css`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/data/css/web.css` & `pygpt_net-2.2.2/src/pygpt_net/data/css/web.css`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/data/css/web.dark.css` & `pygpt_net-2.2.2/src/pygpt_net/data/css/web.dark.css`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/data/css/web.light.css` & `pygpt_net-2.2.2/src/pygpt_net/data/css/web.light.css`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/data/fonts/Lato/Lato-Black.ttf` & `pygpt_net-2.2.2/src/pygpt_net/data/fonts/Lato/Lato-Black.ttf`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/data/fonts/Lato/Lato-BlackItalic.ttf` & `pygpt_net-2.2.2/src/pygpt_net/data/fonts/Lato/Lato-BlackItalic.ttf`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/data/fonts/Lato/Lato-Bold.ttf` & `pygpt_net-2.2.2/src/pygpt_net/data/fonts/Lato/Lato-Bold.ttf`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/data/fonts/Lato/Lato-BoldItalic.ttf` & `pygpt_net-2.2.2/src/pygpt_net/data/fonts/Lato/Lato-BoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/data/fonts/Lato/Lato-Italic.ttf` & `pygpt_net-2.2.2/src/pygpt_net/data/fonts/Lato/Lato-Italic.ttf`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/data/fonts/Lato/Lato-Light.ttf` & `pygpt_net-2.2.2/src/pygpt_net/data/fonts/Lato/Lato-Light.ttf`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/data/fonts/Lato/Lato-LightItalic.ttf` & `pygpt_net-2.2.2/src/pygpt_net/data/fonts/Lato/Lato-LightItalic.ttf`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/data/fonts/Lato/Lato-Regular.ttf` & `pygpt_net-2.2.2/src/pygpt_net/data/fonts/Lato/Lato-Regular.ttf`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/data/fonts/Lato/Lato-Thin.ttf` & `pygpt_net-2.2.2/src/pygpt_net/data/fonts/Lato/Lato-Thin.ttf`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/data/fonts/Lato/Lato-ThinItalic.ttf` & `pygpt_net-2.2.2/src/pygpt_net/data/fonts/Lato/Lato-ThinItalic.ttf`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/data/fonts/Lato/OFL.txt` & `pygpt_net-2.2.2/src/pygpt_net/data/fonts/Lato/OFL.txt`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/data/fonts/MonaspaceArgon/MonaspaceArgon-Bold.otf` & `pygpt_net-2.2.2/src/pygpt_net/data/fonts/MonaspaceArgon/MonaspaceArgon-Bold.otf`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/data/fonts/MonaspaceArgon/MonaspaceArgon-BoldItalic.otf` & `pygpt_net-2.2.2/src/pygpt_net/data/fonts/MonaspaceArgon/MonaspaceArgon-BoldItalic.otf`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/data/fonts/MonaspaceArgon/MonaspaceArgon-Italic.otf` & `pygpt_net-2.2.2/src/pygpt_net/data/fonts/MonaspaceArgon/MonaspaceArgon-Italic.otf`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/data/fonts/MonaspaceArgon/MonaspaceArgon-Regular.otf` & `pygpt_net-2.2.2/src/pygpt_net/data/fonts/MonaspaceArgon/MonaspaceArgon-Regular.otf`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/data/fonts/MonaspaceKrypton/MonaspaceKrypton-Bold.otf` & `pygpt_net-2.2.2/src/pygpt_net/data/fonts/MonaspaceKrypton/MonaspaceKrypton-Bold.otf`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/data/fonts/MonaspaceKrypton/MonaspaceKrypton-BoldItalic.otf` & `pygpt_net-2.2.2/src/pygpt_net/data/fonts/MonaspaceKrypton/MonaspaceKrypton-BoldItalic.otf`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/data/fonts/MonaspaceKrypton/MonaspaceKrypton-Italic.otf` & `pygpt_net-2.2.2/src/pygpt_net/data/fonts/MonaspaceKrypton/MonaspaceKrypton-Italic.otf`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/data/fonts/MonaspaceKrypton/MonaspaceKrypton-Regular.otf` & `pygpt_net-2.2.2/src/pygpt_net/data/fonts/MonaspaceKrypton/MonaspaceKrypton-Regular.otf`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/data/fonts/MonaspaceNeon/MonaspaceNeon-Bold.otf` & `pygpt_net-2.2.2/src/pygpt_net/data/fonts/MonaspaceNeon/MonaspaceNeon-Bold.otf`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/data/fonts/MonaspaceNeon/MonaspaceNeon-BoldItalic.otf` & `pygpt_net-2.2.2/src/pygpt_net/data/fonts/MonaspaceNeon/MonaspaceNeon-BoldItalic.otf`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/data/fonts/MonaspaceNeon/MonaspaceNeon-Italic.otf` & `pygpt_net-2.2.2/src/pygpt_net/data/fonts/MonaspaceNeon/MonaspaceNeon-Italic.otf`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/data/fonts/MonaspaceNeon/MonaspaceNeon-Regular.otf` & `pygpt_net-2.2.2/src/pygpt_net/data/fonts/MonaspaceNeon/MonaspaceNeon-Regular.otf`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/data/fonts/MonaspaceRadon/MonaspaceRadon-Bold.otf` & `pygpt_net-2.2.2/src/pygpt_net/data/fonts/MonaspaceRadon/MonaspaceRadon-Bold.otf`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/data/fonts/MonaspaceRadon/MonaspaceRadon-BoldItalic.otf` & `pygpt_net-2.2.2/src/pygpt_net/data/fonts/MonaspaceRadon/MonaspaceRadon-BoldItalic.otf`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/data/fonts/MonaspaceRadon/MonaspaceRadon-Italic.otf` & `pygpt_net-2.2.2/src/pygpt_net/data/fonts/MonaspaceRadon/MonaspaceRadon-Italic.otf`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/data/fonts/MonaspaceRadon/MonaspaceRadon-Regular.otf` & `pygpt_net-2.2.2/src/pygpt_net/data/fonts/MonaspaceRadon/MonaspaceRadon-Regular.otf`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/data/fonts/MonaspaceXenon/MonaspaceXenon-Bold.otf` & `pygpt_net-2.2.2/src/pygpt_net/data/fonts/MonaspaceXenon/MonaspaceXenon-Bold.otf`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/data/fonts/MonaspaceXenon/MonaspaceXenon-BoldItalic.otf` & `pygpt_net-2.2.2/src/pygpt_net/data/fonts/MonaspaceXenon/MonaspaceXenon-BoldItalic.otf`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/data/fonts/MonaspaceXenon/MonaspaceXenon-Italic.otf` & `pygpt_net-2.2.2/src/pygpt_net/data/fonts/MonaspaceXenon/MonaspaceXenon-Italic.otf`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/data/fonts/MonaspaceXenon/MonaspaceXenon-Regular.otf` & `pygpt_net-2.2.2/src/pygpt_net/data/fonts/MonaspaceXenon/MonaspaceXenon-Regular.otf`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/data/fonts/SpaceMono/OFL.txt` & `pygpt_net-2.2.2/src/pygpt_net/data/fonts/SpaceMono/OFL.txt`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/data/fonts/SpaceMono/SpaceMono-Bold.ttf` & `pygpt_net-2.2.2/src/pygpt_net/data/fonts/SpaceMono/SpaceMono-Bold.ttf`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/data/fonts/SpaceMono/SpaceMono-BoldItalic.ttf` & `pygpt_net-2.2.2/src/pygpt_net/data/fonts/SpaceMono/SpaceMono-BoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/data/fonts/SpaceMono/SpaceMono-Italic.ttf` & `pygpt_net-2.2.2/src/pygpt_net/data/fonts/SpaceMono/SpaceMono-Italic.ttf`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/data/fonts/SpaceMono/SpaceMono-Regular.ttf` & `pygpt_net-2.2.2/src/pygpt_net/data/fonts/SpaceMono/SpaceMono-Regular.ttf`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/data/icon.ico` & `pygpt_net-2.2.2/src/pygpt_net/data/icon.ico`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/data/icon.png` & `pygpt_net-2.2.2/src/pygpt_net/data/icon.png`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/data/icon_tray_busy.ico` & `pygpt_net-2.2.2/src/pygpt_net/data/icon_tray_busy.ico`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/data/icon_tray_error.ico` & `pygpt_net-2.2.2/src/pygpt_net/data/icon_tray_error.ico`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/data/icon_tray_idle.ico` & `pygpt_net-2.2.2/src/pygpt_net/data/icon_tray_idle.ico`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/data/icons/abc.svg` & `pygpt_net-2.2.2/src/pygpt_net/data/icons/abc.svg`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/data/icons/alarm.svg` & `pygpt_net-2.2.2/src/pygpt_net/data/icons/alarm.svg`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/data/icons/apps.svg` & `pygpt_net-2.2.2/src/pygpt_net/data/icons/apps.svg`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/data/icons/build.svg` & `pygpt_net-2.2.2/src/pygpt_net/data/icons/build.svg`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/data/icons/calendar.svg` & `pygpt_net-2.2.2/src/pygpt_net/data/icons/calendar.svg`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/data/icons/chat/audio.png` & `pygpt_net-2.2.2/src/pygpt_net/data/icons/chat/audio.png`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/data/icons/chat/copy.png` & `pygpt_net-2.2.2/src/pygpt_net/data/icons/chat/copy.png`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/data/icons/chat/delete.png` & `pygpt_net-2.2.2/src/pygpt_net/data/icons/chat/delete.png`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/data/icons/chat/edit.png` & `pygpt_net-2.2.2/src/pygpt_net/data/icons/chat/edit.png`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/data/icons/chat/join.png` & `pygpt_net-2.2.2/src/pygpt_net/data/icons/chat/join.png`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/data/icons/chat/reload.png` & `pygpt_net-2.2.2/src/pygpt_net/data/icons/chat/reload.png`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/data/icons/cut.svg` & `pygpt_net-2.2.2/src/pygpt_net/data/icons/cut.svg`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/data/icons/db.svg` & `pygpt_net-2.2.2/src/pygpt_net/data/icons/db.svg`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/data/icons/error.svg` & `pygpt_net-2.2.2/src/pygpt_net/data/icons/error.svg`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/data/icons/hearing.svg` & `pygpt_net-2.2.2/src/pygpt_net/data/icons/hearing.svg`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/data/icons/help.svg` & `pygpt_net-2.2.2/src/pygpt_net/data/icons/help.svg`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/data/icons/info.svg` & `pygpt_net-2.2.2/src/pygpt_net/data/icons/info.svg`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/data/icons/key.svg` & `pygpt_net-2.2.2/src/pygpt_net/data/icons/key.svg`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/data/icons/keyboard.svg` & `pygpt_net-2.2.2/src/pygpt_net/data/icons/keyboard.svg`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/data/icons/language.svg` & `pygpt_net-2.2.2/src/pygpt_net/data/icons/language.svg`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/data/icons/palette.svg` & `pygpt_net-2.2.2/src/pygpt_net/data/icons/palette.svg`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/data/icons/public_filled.svg` & `pygpt_net-2.2.2/src/pygpt_net/data/icons/public_filled.svg`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/data/icons/robot.svg` & `pygpt_net-2.2.2/src/pygpt_net/data/icons/robot.svg`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/data/icons/router.svg` & `pygpt_net-2.2.2/src/pygpt_net/data/icons/router.svg`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/data/icons/sensors.svg` & `pygpt_net-2.2.2/src/pygpt_net/data/icons/sensors.svg`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/data/icons/settings.svg` & `pygpt_net-2.2.2/src/pygpt_net/data/icons/settings.svg`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/data/icons/share.svg` & `pygpt_net-2.2.2/src/pygpt_net/data/icons/share.svg`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/data/icons/view.svg` & `pygpt_net-2.2.2/src/pygpt_net/data/icons/view.svg`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/data/icons/voice.svg` & `pygpt_net-2.2.2/src/pygpt_net/data/icons/voice.svg`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/data/locale/locale.de.ini` & `pygpt_net-2.2.2/src/pygpt_net/data/locale/locale.de.ini`

 * *Files 1% similar despite different names*

```diff
@@ -528,14 +528,16 @@
 settings.agent.mode.desc = Interner Modus für die Verwendung im Agentenmodus (Chat, Vervollständigung, Langchain, Llama_Index usw.)
 settings.agent.goal.notify = Zeige eine Benachrichtigung im Infobereich an, wenn das Ziel erreicht ist.
 settings.agent.idx = Index
 settings.agent.idx.desc = Nur wenn der interne Modus Llama_Index ist (Chat mit Dateien), wählen Sie den Index für die Verwendung im Agentenmodus
 settings.api_endpoint = API-Endpunkt
 settings.api_endpoint.desc = OpenAI-API-Endpunkt-URL, Standard: https://api.openai.com/v1
 settings.api_key = OpenAI API-KEY
+settings.app.env = Anwendungsumgebung (os.environ)
+settings.app.env.desc = Zusätzliche Umgebungsvariablen, die beim Start der Anwendung gesetzt werden sollen
 settings.check_updates = Beim Start nach Updates suchen
 settings.check_updates.bg = Im Hintergrund nach Updates suchen
 settings.context_threshold = Kontextschwelle
 settings.ctx.audio = Audio-Symbol immer anzeigen
 settings.ctx.auto_summary = Kontext automatisch zusammenfassen
 settings.ctx.auto_summary.model = Modell für automatische Zusammenfassung verwendet
 settings.ctx.code_interpreter = Ausgabe des Code-Interpreters anzeigen
```

### Comparing `pygpt_net-2.2.1/src/pygpt_net/data/locale/locale.en.ini` & `pygpt_net-2.2.2/src/pygpt_net/data/locale/locale.en.ini`

 * *Files 0% similar despite different names*

```diff
@@ -662,14 +662,16 @@
 settings.agent.mode.desc = Sub-mode to use in Agent mode (chat, completion, langchain, llama_index, etc.)
 settings.agent.goal.notify = Display a tray notification when the goal is achieved.
 settings.agent.idx = Index to use
 settings.agent.idx.desc = Only if sub-mode is llama_index (Chat with files), choose the index to use in Agent mode
 settings.api_endpoint = API Endpoint
 settings.api_endpoint.desc = OpenAI API endpoint URL, default: https://api.openai.com/v1
 settings.api_key = OpenAI API KEY
+settings.app.env = Application environment (os.environ)
+settings.app.env.desc = Additional environment vars to set on application start
 settings.check_updates = Check for updates on start
 settings.check_updates.bg = Check for updates in background
 settings.cmd.config.collapse = JSON parameters (show/hide)
 settings.cmd.field.enable = Enable: {cmd} (cmd)
 settings.cmd.field.desc = Enable `{cmd}` command execution.
 settings.cmd.field.tooltip = Enable `{cmd}` command execution
 settings.cmd.field.instruction = Instruction for model
```

### Comparing `pygpt_net-2.2.1/src/pygpt_net/data/locale/locale.es.ini` & `pygpt_net-2.2.2/src/pygpt_net/data/locale/locale.es.ini`

 * *Files 0% similar despite different names*

```diff
@@ -527,14 +527,16 @@
 settings.agent.mode.desc = Modo interno para usar en modo Agente (chat, completado, langchain, llama_index, etc.)
 settings.agent.goal.notify = Mostrar una notificación en la bandeja del sistema cuando se logre el objetivo.
 settings.agent.idx = Índice
 settings.agent.idx.desc = Solo si el modo interno es llama_index (Chat con archivos), elige el índice a usar en modo Agente
 settings.api_endpoint = Punto final de la API
 settings.api_endpoint.desc = URL del punto final de la API de OpenAI, por defecto: https://api.openai.com/v1
 settings.api_key = Clave API de OpenAI
+settings.app.env = Entorno de la aplicación (os.environ)
+settings.app.env.desc = Variables de entorno adicionales para configurar en el inicio de la aplicación
 settings.check_updates = Buscar actualizaciones al iniciar
 settings.check_updates.bg = Buscar actualizaciones en segundo plano
 settings.context_threshold = Umbral del contexto
 settings.ctx.audio = Siempre mostrar el ícono de audio
 settings.ctx.auto_summary = Resumen automático del contexto
 settings.ctx.auto_summary.model = Modelo utilizado para el resumen automático
 settings.ctx.code_interpreter = Mostrar salida del intérprete de código
```

### Comparing `pygpt_net-2.2.1/src/pygpt_net/data/locale/locale.fr.ini` & `pygpt_net-2.2.2/src/pygpt_net/data/locale/locale.fr.ini`

 * *Files 0% similar despite different names*

```diff
@@ -527,14 +527,16 @@
 settings.agent.mode.desc = Mode interne à utiliser en mode Agent (chat, complétion, langchain, llama_index, etc.)
 settings.agent.goal.notify = Afficher une notification dans la barre des tâches lorsque l'objectif est atteint.
 settings.agent.idx = Index
 settings.agent.idx.desc = Seulement si le mode interne est llama_index (Chat avec fichiers), choisissez l'index à utiliser en mode Agent
 settings.api_endpoint = Point de terminaison API
 settings.api_endpoint.desc = URL du point de terminaison de l'API OpenAI, par défaut : https://api.openai.com/v1
 settings.api_key = Clé API OpenAI
+settings.app.env = Environnement de l'application (os.environ)
+settings.app.env.desc = Variables d'environnement supplémentaires à définir au démarrage de l'application
 settings.check_updates = Vérifier les mises à jour au démarrage
 settings.check_updates.bg = Vérifier les mises à jour en arrière-plan
 settings.context_threshold = Seuil de contexte
 settings.ctx.audio = Toujours afficher l'icône audio
 settings.ctx.auto_summary = Résumé automatique du contexte
 settings.ctx.auto_summary.model = Modèle utilisé pour le résumé automatique
 settings.ctx.code_interpreter = Afficher la sortie de l'interprèteur de code
```

### Comparing `pygpt_net-2.2.1/src/pygpt_net/data/locale/locale.it.ini` & `pygpt_net-2.2.2/src/pygpt_net/data/locale/locale.it.ini`

 * *Files 1% similar despite different names*

```diff
@@ -528,14 +528,16 @@
 settings.agent.mode.desc = Modalità interna da utilizzare in modalità Agente (chat, completamento, langchain, llama_index, ecc.)
 settings.agent.goal.notify = Visualizza una notifica nella barra delle applicazioni quando l'obiettivo è raggiunto.
 settings.agent.idx = Indice
 settings.agent.idx.desc = Solo se la modalità interna è llama_index (Chat con file), scegli l'indice da utilizzare in modalità Agente
 settings.api_endpoint = Endpoint API
 settings.api_endpoint.desc = URL dell'endpoint API di OpenAI, predefinito: https://api.openai.com/v1
 settings.api_key = OpenAI API KEY
+settings.app.env = Ambiente dell'applicazione (os.environ)
+settings.app.env.desc = Variabili d'ambiente aggiuntive da impostare all'avvio dell'applicazione
 settings.check_updates = Controlla aggiornamenti all'avvio
 settings.check_updates.bg = Controlla gli aggiornamenti in background
 settings.context_threshold = Soglia del contesto
 settings.ctx.audio = Mostra sempre l'icona audio
 settings.ctx.auto_summary = Riassunto automatico del contesto
 settings.ctx.auto_summary.model = Modello utilizzato per riassunto automatico
 settings.ctx.code_interpreter = Mostra l'output dell'interprete del codice
```

### Comparing `pygpt_net-2.2.1/src/pygpt_net/data/locale/locale.pl.ini` & `pygpt_net-2.2.2/src/pygpt_net/data/locale/locale.pl.ini`

 * *Files 0% similar despite different names*

```diff
@@ -528,14 +528,16 @@
 settings.agent.mode.desc = Tryb wewnętrzny do użycia w trybie Agenta (chat, completion, langchain, llama_index itp.)
 settings.agent.goal.notify = Wyświetl powiadomienie w zasobniku systemowym, gdy cel zostanie osiągnięty.
 settings.agent.idx = Indeks
 settings.agent.idx.desc = Tylko jeśli tryb wewnętrzny to llama_index (Czat z plikami), wybierz indeks do użycia w trybie Agenta
 settings.api_endpoint = Punkt końcowy API
 settings.api_endpoint.desc = URL punktu końcowego API OpenAI, domyślnie: https://api.openai.com/v1
 settings.api_key = Klucz API OpenAI
+settings.app.env = Środowisko aplikacji (os.environ)
+settings.app.env.desc = Dodatkowe zmienne środowiskowe do ustawienia przy starcie aplikacji
 settings.check_updates = Sprawdź aktualizacje przy starcie
 settings.check_updates.bg = Sprawdź aktualizacje w tle
 settings.context_threshold = Zarezerwowany kontekst
 settings.ctx.audio = Zawsze pokazuj ikonę audio
 settings.ctx.auto_summary = Kontekst: auto-podsumowanie
 settings.ctx.auto_summary.model = Model używany do auto-podsumowania
 settings.ctx.code_interpreter = Pokaż wyniki interpretacji kodu
```

### Comparing `pygpt_net-2.2.1/src/pygpt_net/data/locale/locale.uk.ini` & `pygpt_net-2.2.2/src/pygpt_net/data/locale/locale.uk.ini`

 * *Files 0% similar despite different names*

```diff
@@ -528,14 +528,16 @@
 settings.agent.mode.desc = Внутрішній режим для використання в режимі Агента (чат, завершення, langchain, llama_index тощо)
 settings.agent.goal.notify = Показати сповіщення в системному треї, коли мета досягнута.
 settings.agent.idx = Індекс
 settings.agent.idx.desc = Тільки якщо внутрішній режим є llama_index (Чат з файлами), виберіть індекс для використання в режимі Агента
 settings.api_endpoint = Кінцева точка API
 settings.api_endpoint.desc = URL кінцевої точки API OpenAI, за замовчуванням: https://api.openai.com/v1
 settings.api_key = OpenAI API КЛЮЧ
+settings.app.env = Оточення додатка (os.environ)
+settings.app.env.desc = Додаткові змінні середовища для встановлення при запуску додатка
 settings.check_updates = Перевіряти оновлення при запуску
 settings.check_updates.bg = Перевіряти оновлення у фоновому режимі
 settings.context_threshold = Поріг контексту
 settings.ctx.audio = Завжди показувати значок аудіо
 settings.ctx.auto_summary = Автоматичне стиснення контексту
 settings.ctx.auto_summary.model = Модель, що використовується для автоматичного стиснення
 settings.ctx.code_interpreter = Показати вивід інтерпретатора коду
```

### Comparing `pygpt_net-2.2.1/src/pygpt_net/data/locale/locale.zh.ini` & `pygpt_net-2.2.2/src/pygpt_net/data/locale/locale.zh.ini`

 * *Files 0% similar despite different names*

```diff
@@ -632,14 +632,16 @@
 settings.agent.mode.desc = 在代理模式下使用的子模式（聊天、完成、langchain、llama_index等）
 settings.agent.goal.notify = 當目標達成時顯示托盤通知。
 settings.agent.idx = 要使用的索引
 settings.agent.idx.desc = 只有在子模式為llama_index（文件聊天）時，選擇在代理模式下使用的索引
 settings.api_endpoint = API端点
 settings.api_endpoint.desc = OpenAI API端点URL，默认为：https://api.openai.com/v1
 settings.api_key = OpenAI API KEY
+settings.app.env = 应用程序环境 (os.environ)
+settings.app.env.desc = 在应用程序启动时要设置的额外环境变量
 settings.check_updates = 啟動時檢查更新
 settings.check_updates.bg = 在後台檢查更新
 settings.context_threshold = 上下文閾值
 settings.ctx.audio = 总是显示音频图标
 settings.ctx.auto_summary = 上下文自動摘要
 settings.ctx.auto_summary.model = 用於自動摘要的模型
 settings.ctx.code_interpreter = 显示代码解释器输出
```

### Comparing `pygpt_net-2.2.1/src/pygpt_net/data/locale/plugin.agent.en.ini` & `pygpt_net-2.2.2/src/pygpt_net/data/locale/plugin.agent.en.ini`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/data/locale/plugin.agent.pl.ini` & `pygpt_net-2.2.2/src/pygpt_net/data/locale/plugin.agent.pl.ini`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/data/locale/plugin.audio_input.en.ini` & `pygpt_net-2.2.2/src/pygpt_net/data/locale/plugin.audio_input.en.ini`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/data/locale/plugin.audio_input.pl.ini` & `pygpt_net-2.2.2/src/pygpt_net/data/locale/plugin.audio_input.pl.ini`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/data/locale/plugin.audio_output.en.ini` & `pygpt_net-2.2.2/src/pygpt_net/data/locale/plugin.audio_output.en.ini`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/data/locale/plugin.audio_output.pl.ini` & `pygpt_net-2.2.2/src/pygpt_net/data/locale/plugin.audio_output.pl.ini`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/data/locale/plugin.cmd_api.en.ini` & `pygpt_net-2.2.2/src/pygpt_net/data/locale/plugin.cmd_api.en.ini`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/data/locale/plugin.cmd_api.pl.ini` & `pygpt_net-2.2.2/src/pygpt_net/data/locale/plugin.cmd_api.pl.ini`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/data/locale/plugin.cmd_code_interpreter.en.ini` & `pygpt_net-2.2.2/src/pygpt_net/data/locale/plugin.cmd_code_interpreter.en.ini`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/data/locale/plugin.cmd_code_interpreter.pl.ini` & `pygpt_net-2.2.2/src/pygpt_net/data/locale/plugin.cmd_code_interpreter.pl.ini`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/data/locale/plugin.cmd_custom.pl.ini` & `pygpt_net-2.2.2/src/pygpt_net/data/locale/plugin.cmd_custom.pl.ini`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/data/locale/plugin.cmd_files.en.ini` & `pygpt_net-2.2.2/src/pygpt_net/data/locale/plugin.cmd_files.en.ini`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/data/locale/plugin.cmd_files.pl.ini` & `pygpt_net-2.2.2/src/pygpt_net/data/locale/plugin.cmd_files.pl.ini`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/data/locale/plugin.cmd_history.en.ini` & `pygpt_net-2.2.2/src/pygpt_net/data/locale/plugin.cmd_history.en.ini`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/data/locale/plugin.cmd_history.pl.ini` & `pygpt_net-2.2.2/src/pygpt_net/data/locale/plugin.cmd_history.pl.ini`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/data/locale/plugin.cmd_serial.en.ini` & `pygpt_net-2.2.2/src/pygpt_net/data/locale/plugin.cmd_serial.en.ini`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/data/locale/plugin.cmd_serial.pl.ini` & `pygpt_net-2.2.2/src/pygpt_net/data/locale/plugin.cmd_serial.pl.ini`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/data/locale/plugin.cmd_web.en.ini` & `pygpt_net-2.2.2/src/pygpt_net/data/locale/plugin.cmd_web.en.ini`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/data/locale/plugin.cmd_web.pl.ini` & `pygpt_net-2.2.2/src/pygpt_net/data/locale/plugin.cmd_web.pl.ini`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/data/locale/plugin.crontab.en.ini` & `pygpt_net-2.2.2/src/pygpt_net/data/locale/plugin.crontab.en.ini`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/data/locale/plugin.crontab.pl.ini` & `pygpt_net-2.2.2/src/pygpt_net/data/locale/plugin.crontab.pl.ini`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/data/locale/plugin.idx_llama_index.en.ini` & `pygpt_net-2.2.2/src/pygpt_net/data/locale/plugin.idx_llama_index.en.ini`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/data/locale/plugin.idx_llama_index.pl.ini` & `pygpt_net-2.2.2/src/pygpt_net/data/locale/plugin.idx_llama_index.pl.ini`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/data/locale/plugin.openai_vision.en.ini` & `pygpt_net-2.2.2/src/pygpt_net/data/locale/plugin.openai_vision.en.ini`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/data/locale/plugin.openai_vision.pl.ini` & `pygpt_net-2.2.2/src/pygpt_net/data/locale/plugin.openai_vision.pl.ini`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/data/locale/plugin.real_time.en.ini` & `pygpt_net-2.2.2/src/pygpt_net/data/locale/plugin.real_time.en.ini`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/data/locale/plugin.real_time.pl.ini` & `pygpt_net-2.2.2/src/pygpt_net/data/locale/plugin.real_time.pl.ini`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/data/logo.png` & `pygpt_net-2.2.2/src/pygpt_net/data/logo.png`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/data/prompts.csv` & `pygpt_net-2.2.2/src/pygpt_net/data/prompts.csv`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/data/win32/README.rtf` & `pygpt_net-2.2.2/src/pygpt_net/data/win32/README.rtf`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/data/win32/USER-LICENSE.rtf` & `pygpt_net-2.2.2/src/pygpt_net/data/win32/USER-LICENSE.rtf`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/data/win32/pygpt.aip` & `pygpt_net-2.2.2/src/pygpt_net/data/win32/pygpt.aip`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/icons.qrc` & `pygpt_net-2.2.2/src/pygpt_net/icons.qrc`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/icons_rc.py` & `pygpt_net-2.2.2/src/pygpt_net/icons_rc.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/item/assistant.py` & `pygpt_net-2.2.2/src/pygpt_net/item/assistant.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/item/attachment.py` & `pygpt_net-2.2.2/src/pygpt_net/item/attachment.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/item/calendar_note.py` & `pygpt_net-2.2.2/src/pygpt_net/item/calendar_note.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/item/ctx.py` & `pygpt_net-2.2.2/src/pygpt_net/item/ctx.py`

 * *Files 0% similar despite different names*

```diff
@@ -54,14 +54,15 @@
         self.is_vision = False
         self.idx = 0
         self.first = False
         self.tool_calls = []  # API tool calls
         self.index_meta = {}  # llama-index metadata ctx used
         self.doc_ids = []  # document ids
         self.prev_ctx = None  # previous context (reply output)
+        self.stopped = False  # run stopped
 
     def clear_reply(self):
         """Clear current reply output"""
         if self.reply:
             self.urls = []
 
     def from_previous(self):
```

### Comparing `pygpt_net-2.2.1/src/pygpt_net/item/index.py` & `pygpt_net-2.2.2/src/pygpt_net/item/index.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/item/mode.py` & `pygpt_net-2.2.2/src/pygpt_net/item/mode.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/item/model.py` & `pygpt_net-2.2.2/src/pygpt_net/item/model.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/item/notepad.py` & `pygpt_net-2.2.2/src/pygpt_net/item/notepad.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/item/preset.py` & `pygpt_net-2.2.2/src/pygpt_net/item/preset.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/launcher.py` & `pygpt_net-2.2.2/src/pygpt_net/launcher.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/migrations/Version20231227152900.py` & `pygpt_net-2.2.2/src/pygpt_net/migrations/Version20231227152900.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/migrations/Version20231230095000.py` & `pygpt_net-2.2.2/src/pygpt_net/migrations/Version20231230095000.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/migrations/Version20231231230000.py` & `pygpt_net-2.2.2/src/pygpt_net/migrations/Version20231231230000.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/migrations/Version20240106060000.py` & `pygpt_net-2.2.2/src/pygpt_net/migrations/Version20240106060000.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/migrations/Version20240107060000.py` & `pygpt_net-2.2.2/src/pygpt_net/migrations/Version20240107060000.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/migrations/Version20240222160000.py` & `pygpt_net-2.2.2/src/pygpt_net/migrations/Version20240222160000.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/migrations/Version20240223050000.py` & `pygpt_net-2.2.2/src/pygpt_net/migrations/Version20240223050000.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/migrations/Version20240303190000.py` & `pygpt_net-2.2.2/src/pygpt_net/migrations/Version20240303190000.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/migrations/Version20240408180000.py` & `pygpt_net-2.2.2/src/pygpt_net/migrations/Version20240408180000.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/migrations/Version20240426050000.py` & `pygpt_net-2.2.2/src/pygpt_net/migrations/Version20240426050000.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/migrations/__init__.py` & `pygpt_net-2.2.2/src/pygpt_net/migrations/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/migrations/base.py` & `pygpt_net-2.2.2/src/pygpt_net/migrations/base.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/plugin/agent/__init__.py` & `pygpt_net-2.2.2/src/pygpt_net/plugin/agent/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/plugin/audio_input/__init__.py` & `pygpt_net-2.2.2/src/pygpt_net/plugin/audio_input/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/plugin/audio_input/simple.py` & `pygpt_net-2.2.2/src/pygpt_net/plugin/audio_input/simple.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/plugin/audio_input/worker.py` & `pygpt_net-2.2.2/src/pygpt_net/plugin/audio_input/worker.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/plugin/audio_output/__init__.py` & `pygpt_net-2.2.2/src/pygpt_net/plugin/audio_output/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/plugin/audio_output/worker.py` & `pygpt_net-2.2.2/src/pygpt_net/plugin/audio_output/worker.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/plugin/base.py` & `pygpt_net-2.2.2/src/pygpt_net/plugin/base.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/plugin/cmd_api/__init__.py` & `pygpt_net-2.2.2/src/pygpt_net/plugin/cmd_api/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/plugin/cmd_api/worker.py` & `pygpt_net-2.2.2/src/pygpt_net/plugin/cmd_api/worker.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/plugin/cmd_code_interpreter/__init__.py` & `pygpt_net-2.2.2/src/pygpt_net/plugin/cmd_code_interpreter/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/plugin/cmd_code_interpreter/runner.py` & `pygpt_net-2.2.2/src/pygpt_net/plugin/cmd_code_interpreter/runner.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/plugin/cmd_code_interpreter/worker.py` & `pygpt_net-2.2.2/src/pygpt_net/plugin/cmd_code_interpreter/worker.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/plugin/cmd_custom/__init__.py` & `pygpt_net-2.2.2/src/pygpt_net/plugin/cmd_custom/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/plugin/cmd_custom/worker.py` & `pygpt_net-2.2.2/src/pygpt_net/plugin/cmd_custom/worker.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/plugin/cmd_files/__init__.py` & `pygpt_net-2.2.2/src/pygpt_net/plugin/cmd_files/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/plugin/cmd_files/worker.py` & `pygpt_net-2.2.2/src/pygpt_net/plugin/cmd_files/worker.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/plugin/cmd_history/__init__.py` & `pygpt_net-2.2.2/src/pygpt_net/plugin/cmd_history/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/plugin/cmd_history/worker.py` & `pygpt_net-2.2.2/src/pygpt_net/plugin/cmd_history/worker.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/plugin/cmd_serial/__init__.py` & `pygpt_net-2.2.2/src/pygpt_net/plugin/cmd_serial/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/plugin/cmd_serial/worker.py` & `pygpt_net-2.2.2/src/pygpt_net/plugin/cmd_serial/worker.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/plugin/cmd_web/__init__.py` & `pygpt_net-2.2.2/src/pygpt_net/plugin/cmd_web/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/plugin/cmd_web/websearch.py` & `pygpt_net-2.2.2/src/pygpt_net/plugin/cmd_web/websearch.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/plugin/cmd_web/worker.py` & `pygpt_net-2.2.2/src/pygpt_net/plugin/cmd_web/worker.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/plugin/crontab/__init__.py` & `pygpt_net-2.2.2/src/pygpt_net/plugin/crontab/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/plugin/extra_prompt/__init__.py` & `pygpt_net-2.2.2/src/pygpt_net/plugin/extra_prompt/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/plugin/idx_llama_index/__init__.py` & `pygpt_net-2.2.2/src/pygpt_net/plugin/idx_llama_index/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/plugin/idx_llama_index/worker.py` & `pygpt_net-2.2.2/src/pygpt_net/plugin/idx_llama_index/worker.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/plugin/openai_dalle/__init__.py` & `pygpt_net-2.2.2/src/pygpt_net/plugin/openai_dalle/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/plugin/openai_vision/__init__.py` & `pygpt_net-2.2.2/src/pygpt_net/plugin/openai_vision/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/plugin/real_time/__init__.py` & `pygpt_net-2.2.2/src/pygpt_net/plugin/real_time/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/provider/audio_input/base.py` & `pygpt_net-2.2.2/src/pygpt_net/provider/audio_input/base.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/provider/audio_input/bing_speech_recognition.py` & `pygpt_net-2.2.2/src/pygpt_net/provider/audio_input/bing_speech_recognition.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/provider/audio_input/google_cloud_speech_recognition.py` & `pygpt_net-2.2.2/src/pygpt_net/provider/audio_input/google_cloud_speech_recognition.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/provider/audio_input/google_speech_recognition.py` & `pygpt_net-2.2.2/src/pygpt_net/provider/audio_input/google_speech_recognition.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/provider/audio_input/openai_whisper.py` & `pygpt_net-2.2.2/src/pygpt_net/provider/audio_input/openai_whisper.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/provider/audio_input/openai_whisper_local.py` & `pygpt_net-2.2.2/src/pygpt_net/provider/audio_input/openai_whisper_local.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/provider/audio_output/base.py` & `pygpt_net-2.2.2/src/pygpt_net/provider/audio_output/base.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/provider/audio_output/eleven_labs.py` & `pygpt_net-2.2.2/src/pygpt_net/provider/audio_output/eleven_labs.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/provider/audio_output/google_tts.py` & `pygpt_net-2.2.2/src/pygpt_net/provider/audio_output/google_tts.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/provider/audio_output/ms_azure_tts.py` & `pygpt_net-2.2.2/src/pygpt_net/provider/audio_output/ms_azure_tts.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/provider/audio_output/openai_tts.py` & `pygpt_net-2.2.2/src/pygpt_net/provider/audio_output/openai_tts.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/provider/core/assistant/base.py` & `pygpt_net-2.2.2/src/pygpt_net/provider/core/assistant/base.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/provider/core/assistant/json_file.py` & `pygpt_net-2.2.2/src/pygpt_net/provider/core/assistant/json_file.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/provider/core/assistant_file/base.py` & `pygpt_net-2.2.2/src/pygpt_net/provider/core/assistant_file/base.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/provider/core/assistant_file/db_sqlite/__init__.py` & `pygpt_net-2.2.2/src/pygpt_net/provider/core/assistant_file/db_sqlite/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/provider/core/assistant_file/db_sqlite/patch.py` & `pygpt_net-2.2.2/src/pygpt_net/provider/core/assistant_file/db_sqlite/patch.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/provider/core/assistant_file/db_sqlite/storage.py` & `pygpt_net-2.2.2/src/pygpt_net/provider/core/assistant_file/db_sqlite/storage.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/provider/core/assistant_file/db_sqlite/utils.py` & `pygpt_net-2.2.2/src/pygpt_net/provider/core/assistant_file/db_sqlite/utils.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/provider/core/assistant_store/base.py` & `pygpt_net-2.2.2/src/pygpt_net/provider/core/assistant_store/base.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/provider/core/assistant_store/db_sqlite/__init__.py` & `pygpt_net-2.2.2/src/pygpt_net/provider/core/assistant_store/db_sqlite/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/provider/core/assistant_store/db_sqlite/patch.py` & `pygpt_net-2.2.2/src/pygpt_net/provider/core/assistant_store/db_sqlite/patch.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/provider/core/assistant_store/db_sqlite/storage.py` & `pygpt_net-2.2.2/src/pygpt_net/provider/core/assistant_store/db_sqlite/storage.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/provider/core/assistant_store/db_sqlite/utils.py` & `pygpt_net-2.2.2/src/pygpt_net/provider/core/assistant_store/db_sqlite/utils.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/provider/core/assistant_store/json_file.py` & `pygpt_net-2.2.2/src/pygpt_net/provider/core/assistant_store/json_file.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/provider/core/attachment/base.py` & `pygpt_net-2.2.2/src/pygpt_net/provider/core/attachment/base.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/provider/core/attachment/json_file.py` & `pygpt_net-2.2.2/src/pygpt_net/provider/core/attachment/json_file.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/provider/core/calendar/base.py` & `pygpt_net-2.2.2/src/pygpt_net/provider/core/calendar/base.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/provider/core/calendar/db_sqlite/__init__.py` & `pygpt_net-2.2.2/src/pygpt_net/provider/core/calendar/db_sqlite/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/provider/core/calendar/db_sqlite/patch.py` & `pygpt_net-2.2.2/src/pygpt_net/provider/core/calendar/db_sqlite/patch.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/provider/core/calendar/db_sqlite/storage.py` & `pygpt_net-2.2.2/src/pygpt_net/provider/core/calendar/db_sqlite/storage.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/provider/core/config/base.py` & `pygpt_net-2.2.2/src/pygpt_net/provider/core/config/base.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/provider/core/config/json_file.py` & `pygpt_net-2.2.2/src/pygpt_net/provider/core/config/json_file.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/provider/core/config/patch.py` & `pygpt_net-2.2.2/src/pygpt_net/provider/core/config/patch.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # -*- coding: utf-8 -*-
 # ================================================== #
 # This file is a part of PYGPT package               #
 # Website: https://pygpt.net                         #
 # GitHub:  https://github.com/szczyglis-dev/py-gpt   #
 # MIT License                                        #
 # Created By  : Marcin Szczygliński                  #
-# Updated Date: 2024.04.26 23:00:00                  #
+# Updated Date: 2024.04.29 07:00:00                  #
 # ================================================== #
 
 import copy
 import os
 
 from packaging.version import parse as parse_version, Version
 
@@ -1404,14 +1404,21 @@
             # < 2.1.79
             if old < parse_version("2.1.79"):
                 print("Migrating config from < 2.1.79...")
                 if 'assistant.store.hide_threads' not in data:
                     data["assistant.store.hide_threads"] = True
                 updated = True
 
+            # < 2.2.2
+            if old < parse_version("2.2.2"):
+                print("Migrating config from < 2.2.2...")
+                if 'app.env' not in data:
+                    data["app.env"] = []
+                updated = True
+
         # update file
         migrated = False
         if updated:
             data = dict(sorted(data.items()))
             self.window.core.config.data = data
             self.window.core.config.save()
             migrated = True
```

### Comparing `pygpt_net-2.2.1/src/pygpt_net/provider/core/ctx/base.py` & `pygpt_net-2.2.2/src/pygpt_net/provider/core/ctx/base.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/provider/core/ctx/db_sqlite/__init__.py` & `pygpt_net-2.2.2/src/pygpt_net/provider/core/ctx/db_sqlite/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/provider/core/ctx/db_sqlite/patch.py` & `pygpt_net-2.2.2/src/pygpt_net/provider/core/ctx/db_sqlite/patch.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/provider/core/ctx/db_sqlite/storage.py` & `pygpt_net-2.2.2/src/pygpt_net/provider/core/ctx/db_sqlite/storage.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/provider/core/ctx/db_sqlite/utils.py` & `pygpt_net-2.2.2/src/pygpt_net/provider/core/ctx/db_sqlite/utils.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/provider/core/ctx/json_file.py` & `pygpt_net-2.2.2/src/pygpt_net/provider/core/ctx/json_file.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/provider/core/history/base.py` & `pygpt_net-2.2.2/src/pygpt_net/provider/core/history/base.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/provider/core/history/patch.py` & `pygpt_net-2.2.2/src/pygpt_net/provider/core/history/patch.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/provider/core/history/txt_file.py` & `pygpt_net-2.2.2/src/pygpt_net/provider/core/history/txt_file.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/provider/core/index/base.py` & `pygpt_net-2.2.2/src/pygpt_net/provider/core/index/base.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/provider/core/index/db_sqlite/__init__.py` & `pygpt_net-2.2.2/src/pygpt_net/provider/core/index/db_sqlite/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/provider/core/index/db_sqlite/patch.py` & `pygpt_net-2.2.2/src/pygpt_net/provider/core/index/db_sqlite/patch.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/provider/core/index/db_sqlite/storage.py` & `pygpt_net-2.2.2/src/pygpt_net/provider/core/index/db_sqlite/storage.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/provider/core/index/db_sqlite/utils.py` & `pygpt_net-2.2.2/src/pygpt_net/provider/core/index/db_sqlite/utils.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/provider/core/index/json_file.py` & `pygpt_net-2.2.2/src/pygpt_net/provider/core/index/json_file.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/provider/core/index/patch.py` & `pygpt_net-2.2.2/src/pygpt_net/provider/core/index/patch.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/provider/core/mode/base.py` & `pygpt_net-2.2.2/src/pygpt_net/provider/core/mode/base.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/provider/core/mode/json_file.py` & `pygpt_net-2.2.2/src/pygpt_net/provider/core/mode/json_file.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/provider/core/mode/patch.py` & `pygpt_net-2.2.2/src/pygpt_net/provider/core/mode/patch.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/provider/core/model/base.py` & `pygpt_net-2.2.2/src/pygpt_net/provider/core/model/base.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/provider/core/model/json_file.py` & `pygpt_net-2.2.2/src/pygpt_net/provider/core/model/json_file.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/provider/core/model/patch.py` & `pygpt_net-2.2.2/src/pygpt_net/provider/core/model/patch.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/provider/core/notepad/base.py` & `pygpt_net-2.2.2/src/pygpt_net/provider/core/notepad/base.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/provider/core/notepad/db_sqlite/__init__.py` & `pygpt_net-2.2.2/src/pygpt_net/provider/core/notepad/db_sqlite/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/provider/core/notepad/db_sqlite/patch.py` & `pygpt_net-2.2.2/src/pygpt_net/provider/core/notepad/db_sqlite/patch.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/provider/core/notepad/db_sqlite/storage.py` & `pygpt_net-2.2.2/src/pygpt_net/provider/core/notepad/db_sqlite/storage.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/provider/core/notepad/json_file.py` & `pygpt_net-2.2.2/src/pygpt_net/provider/core/notepad/json_file.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/provider/core/plugin_preset/base.py` & `pygpt_net-2.2.2/src/pygpt_net/provider/core/plugin_preset/base.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/provider/core/plugin_preset/json_file.py` & `pygpt_net-2.2.2/src/pygpt_net/provider/core/plugin_preset/json_file.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/provider/core/plugin_preset/patch.py` & `pygpt_net-2.2.2/src/pygpt_net/provider/core/plugin_preset/patch.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/provider/core/preset/base.py` & `pygpt_net-2.2.2/src/pygpt_net/provider/core/preset/base.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/provider/core/preset/json_file.py` & `pygpt_net-2.2.2/src/pygpt_net/provider/core/preset/json_file.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/provider/core/preset/patch.py` & `pygpt_net-2.2.2/src/pygpt_net/provider/core/preset/patch.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/provider/gpt/__init__.py` & `pygpt_net-2.2.2/src/pygpt_net/provider/gpt/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/provider/gpt/assistants.py` & `pygpt_net-2.2.2/src/pygpt_net/provider/gpt/assistants.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/provider/gpt/chat.py` & `pygpt_net-2.2.2/src/pygpt_net/provider/gpt/chat.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/provider/gpt/completion.py` & `pygpt_net-2.2.2/src/pygpt_net/provider/gpt/completion.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/provider/gpt/image.py` & `pygpt_net-2.2.2/src/pygpt_net/provider/gpt/image.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/provider/gpt/summarizer.py` & `pygpt_net-2.2.2/src/pygpt_net/provider/gpt/summarizer.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/provider/gpt/vision.py` & `pygpt_net-2.2.2/src/pygpt_net/provider/gpt/vision.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/provider/gpt/worker/assistants.py` & `pygpt_net-2.2.2/src/pygpt_net/provider/gpt/worker/assistants.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,34 +2,38 @@
 # -*- coding: utf-8 -*-
 # ================================================== #
 # This file is a part of PYGPT package               #
 # Website: https://pygpt.net                         #
 # GitHub:  https://github.com/szczyglis-dev/py-gpt   #
 # MIT License                                        #
 # Created By  : Marcin Szczygliński                  #
-# Updated Date: 2024.04.28 07:00:00                  #
+# Updated Date: 2024.04.29 07:00:00                  #
 # ================================================== #
 
 from openai import AssistantEventHandler
 
 from PySide6.QtCore import QObject, Signal, QRunnable, Slot
 from typing_extensions import override
 
 from pygpt_net.item.ctx import CtxItem
 
 
 class AssistantsWorker:
+    CHUNK_TYPE_MSG = 1  # last chunk = message
+    CHUNK_TYPE_TOOL = 0  # last chunk = tool
+
     def __init__(self, window=None):
         """
         Assistants Worker (async)
 
         :param window: Window instance
         """
         self.window = window
         self.tool_output = ""
+        self.last_chunk_type = self.CHUNK_TYPE_MSG  # msg or tool
 
     def create_run(
             self,
             ctx: CtxItem,
             thread_id: str,
             assistant_id: str,
             system_prompt: str
@@ -114,23 +118,51 @@
         worker.signals.stream_text_delta.connect(self.handle_text_delta)
         worker.signals.stream_end.connect(self.handle_end)
         worker.signals.stream_tool_call_created.connect(self.handle_tool_call_created)
         worker.signals.stream_tool_call_delta.connect(self.handle_tool_call_delta)
         worker.signals.stream_tool_call_done.connect(self.handle_tool_call_done)
         worker.signals.stream_message_done.connect(self.handle_message_done)
         worker.signals.stream_run_step_created.connect(self.handle_run_step_created)
+        worker.signals.stream_run_step_done.connect(self.handle_run_step_done)
+        worker.signals.stream_run_created.connect(self.handle_run_created)
 
     def is_show_tool_output(self) -> bool:
         """
         Return True if show tool output
 
         :return: bool
         """
         return self.window.core.config.get('ctx.code_interpreter', False)
 
+    def begin_chunks(self, ctx: CtxItem):
+        """
+        Begin chunks stream output
+
+        :param ctx: context item
+        """
+        self.window.controller.chat.render.stream_begin()
+        self.window.controller.assistant.threads.handle_stream_begin(ctx)
+        self.window.controller.chat.render.append_chunk(
+            ctx,
+            "",
+            True,
+        )  # only begin chunks
+
+    def reset_tool_output(self):
+        """Reset tool output"""
+        self.tool_output = ""
+
+    def has_tool_output(self) -> bool:
+        """
+        Return True if has tool output
+
+        :return: bool
+        """
+        return self.tool_output is not None and self.tool_output != ""
+
     def append_chunk(self, ctx: CtxItem, chunk: str, begin: bool = False):
         """
         Append chunk to context output
 
         :param ctx: context item
         :param chunk: chunk
         :param begin: stream text begin
@@ -138,152 +170,222 @@
         if ctx.output is None:
             ctx.output = ""
         if chunk is not None:
             ctx.output += chunk
         self.window.controller.chat.render.append_chunk(
             ctx,
             chunk,
-            begin,
+            False,
         )
 
+    def log(self, message: str):
+        """
+        Log assistant message
+
+        :param message: message
+        """
+        self.window.controller.assistant.threads.log(message)
+
     @Slot(object)
     def handle_text_created(self, ctx: CtxItem):
         """
         Handle thread text created signal
 
         :param ctx: context item
         """
-        if (ctx.output != "" and ctx.output is not None) or self.tool_output != "":
+        self.log("STREAM: text created")
+        if ctx.stopped:
+            self.log("STREAM: ignoring: stopped")
+            return
+        if (ctx.output != "" and ctx.output is not None) or self.has_tool_output():
             return  # append to existing output
-        self.window.controller.chat.render.stream_begin()
-        self.window.controller.assistant.threads.handle_stream_begin(ctx)
 
     @Slot(object, object)
     def handle_text_delta(self, ctx: CtxItem, delta, begin):
         """
         Handle thread text delta signal
 
         :param ctx: context item
         :param delta: delta
         :param begin: stream text begin
         """
+        if ctx.stopped:
+            return
+        # self.window.controller.assistant.threads.log("STREAM: text delta")
         if ctx.output_tokens is None:
             ctx.output_tokens = 0
         ctx.output_tokens += 1  # tokens++
         self.append_chunk(ctx, delta.value, begin)
+        self.last_chunk_type = self.CHUNK_TYPE_MSG
+        # self.log("STREAM: chunk: msg text")
 
     @Slot(object)
     def handle_end(self, ctx: CtxItem):
         """
         Handle thread end signal
 
         :param ctx: context item
         """
-        self.tool_output = ""
+        self.log("STREAM: end")
+        if ctx.stopped:
+            return
+        self.reset_tool_output()
         self.window.controller.chat.render.stream_end()
         self.window.controller.assistant.threads.handle_output_message(ctx, stream=True)
 
-    @Slot(object, object)
-    def handle_tool_call_created(self, ctx: CtxItem, tool_call):
+    @Slot(object, object, bool)
+    def handle_tool_call_created(self, ctx: CtxItem, tool_call, begin):
         """
         Handle thread tool call created signal
 
         :param ctx: context item
         :param tool_call: tool call
+        :param begin: stream text begin
         """
+        self.log("STREAM: tool call created: {}".format(tool_call.type))
+        if ctx.stopped:
+            self.log("STREAM: ignoring: stopped")
+            return
         if self.is_show_tool_output():
-            self.tool_output = ""
+            self.reset_tool_output()
 
     @Slot(object, object, bool)
     def handle_tool_call_delta(self, ctx: CtxItem, delta, begin):
         """
         Handle thread tool call delta signal
 
         :param ctx: context item
         :param delta: delta
         :param begin: stream text begin
         """
+        if ctx.stopped:
+            return
+        # self.log("STREAM: tool call delta")
         if self.is_show_tool_output():
             if delta.type == 'code_interpreter':
+                # begin code block
+                if begin:
+                    self.log("STREAM: tool output: code_interpreter: begin")
+                    self.append_chunk(ctx, "\n\n**Code interpreter**\n```python\n", begin=False)
+
+                # input
                 if delta.code_interpreter.input:
                     if delta.code_interpreter.input is not None:
-                        if self.tool_output == "":
-                            self.window.controller.chat.render.stream_begin()
-                            self.window.controller.assistant.threads.handle_stream_begin(ctx)
-                            self.append_chunk(ctx, "\n\n**Code interpreter**\n```python\n", begin=begin)
                         self.tool_output += delta.code_interpreter.input
                         self.append_chunk(ctx, delta.code_interpreter.input)
+                        self.last_chunk_type = self.CHUNK_TYPE_TOOL
+                        # self.log("STREAM: chunk: code_interpreter: input")
 
+                # output
                 if delta.code_interpreter.outputs:
                     header = False
                     for output in delta.code_interpreter.outputs:
                         if output.type == "logs":
                             if not header:
+                                self.log("STREAM: tool output: code_interpreter: log begin")
                                 self.append_chunk(ctx, "\n\n-------\nOutput:\n")
+                                self.last_chunk_type = self.CHUNK_TYPE_TOOL
                                 header = True
                             chunk = output.logs
                             if output.logs is not None:
                                 self.append_chunk(ctx, "\n" + chunk)
+                                self.last_chunk_type = self.CHUNK_TYPE_TOOL
+                                # self.log("STREAM: chunk: code_interpreter: logs")
 
     @Slot(object, object, bool)
     def handle_tool_call_done(self, ctx: CtxItem, tool_call, begin):
         """
         Handle thread tool call done signal
 
         :param ctx: context item
         :param tool_call: tool call
         :param begin: stream text begin
         """
+        self.log("STREAM: tool call done: {}".format(tool_call.type))
+        if ctx.stopped:
+            self.log("STREAM: ignoring: stopped")
+            return
         if self.is_show_tool_output():
-            if self.tool_output is not None and self.tool_output != "":
+            if self.has_tool_output() and self.last_chunk_type == self.CHUNK_TYPE_TOOL:
                 self.append_chunk(ctx, "\n```\n")
 
     @Slot(object, object)
     def handle_message_done(self, ctx: CtxItem, message):
         """
         Handle thread message done signal
 
         :param ctx: context item
         :param message: message
         """
+        self.log("STREAM: message done")
+        if ctx.stopped:
+            self.log("STREAM: ignoring: stopped")
+            return
         self.window.controller.assistant.threads.handle_message_data(
             ctx,
             message,
             stream=True,
         )  # handle img, files, etc.
 
-    @Slot(object, object)
-    def handle_run_step_created(self, ctx: CtxItem, run_step):
+    @Slot(object, object, int)
+    def handle_run_step_created(self, ctx: CtxItem, run_step, step_idx: int):
         """
         Handle thread run step created signal
 
         :param ctx: context item
         :param run_step: run step
+        :param step_idx: step index
         """
+        self.log("STREAM: run step created: {}, idx: {}".format(run_step.id, step_idx))
+        if ctx.stopped:
+            self.log("STREAM: ignoring: stopped")
+            return
         ctx.run_id = run_step.run_id
+        self.window.controller.assistant.threads.handle_run_step_created(ctx, stream=True)
+        if step_idx == 0:
+            self.log("STREAM: run created: {}".format(ctx.run_id))
+            self.log("STREAM: begin chunks...")
+            self.begin_chunks(ctx)
+
+    @Slot(object, object, int)
+    def handle_run_step_done(self, ctx: CtxItem, run_step, step_idx: int):
+        """
+        Handle thread run step created signal
+
+        :param ctx: context item
+        :param run_step: run step
+        :param step_idx: step index
+        """
+        self.log("STREAM: run step done: {}, idx: {}".format(run_step.id, step_idx))
+        if ctx.stopped:
+            self.log("STREAM: ignoring: stopped")
+            return
 
     @Slot(object, object)
     def handle_error(self, ctx: CtxItem, err: any):
         """
         Handle thread error signal
 
         :param ctx: context item
         :param err: error message
         """
+        self.log("STREAM: error: {}".format(err))
         self.window.controller.assistant.threads.handle_run_error(ctx, err)
 
     @Slot(object, object, bool)
     def handle_run_created(self, ctx: CtxItem, run, stream=False):
         """
         Handle thread finished signal
 
         :param ctx: context item
         :param run
         :param stream: stream mode
         """
+        if not stream:
+            self.log("STREAM: run created: {}".format(run.id))
         self.window.controller.assistant.threads.handle_run_created(
             ctx,
             run,
             stream=stream
         )
 
 
@@ -294,38 +396,46 @@
             signals: QObject = None,
             ctx: CtxItem = None
 
     ):
         super().__init__()
         self.signals = signals
         self.ctx = ctx
-        self.begin = False
+        self.text_begin = False
         self.tool_begin = False
         self.stream_started = False
+        self.step_idx = 0
         
     @override
     def on_text_created(self, text) -> None:
         """Callback that is fired when a text content block is created"""
         # print(f"\nassistant > ", end="", flush=True)
         if not self.stream_started:
-            self.begin = True
+            self.text_begin = True
         self.stream_started = True
         self.signals.stream_text_created.emit(self.ctx)
 
     @override
     def on_text_delta(self, delta, snapshot):
         """Callback that is fired whenever a message delta is returned from the API"""
         # print(delta.value, end="", flush=True)
-        self.signals.stream_text_delta.emit(self.ctx, delta, self.begin)
-        self.begin = False
+        self.signals.stream_text_delta.emit(self.ctx, delta, self.text_begin)
+        self.text_begin = False
 
     @override
     def on_run_step_created(self, run_step) -> None:
         """Callback that is fired when a run step is created"""
-        self.signals.stream_run_step_created.emit(self.ctx, run_step)
+        self.tool_begin = False  # reset
+        self.signals.stream_run_step_created.emit(self.ctx, run_step, self.step_idx)
+        self.step_idx += 1
+
+    @override
+    def on_run_step_done(self, run_step):
+        """Fires when run completed."""
+        self.signals.stream_run_step_done.emit(self.ctx, run_step, self.step_idx)
 
     @override
     def on_text_done(self, text):
         """Callback that is fired when a text content block is finished"""
         pass
 
     @override
@@ -349,24 +459,25 @@
         """Fires if the request times out"""
         self.signals.error.emit(self.ctx,  "Timeout")
 
     @override
     def on_tool_call_created(self, tool_call):
         """Callback that is fired when a tool call is created"""
         # print(f"\nassistant > {tool_call.type}\n", flush=True)
-        if not self.stream_started:
-            self.tool_begin = True
-        self.stream_started = True
-        self.signals.stream_tool_call_created.emit(self.ctx, tool_call)
+        self.tool_begin = False  # reset
+        self.signals.stream_tool_call_created.emit(self.ctx, tool_call, self.tool_begin)
 
     @override
     def on_tool_call_delta(self, delta, snapshot):
         """Callback that is fired when a tool call delta is encountered"""
-        self.signals.stream_tool_call_delta.emit(self.ctx, delta, self.tool_begin)
-        self.tool_begin = False
+        begin = True
+        if self.tool_begin:
+            begin = False
+        self.signals.stream_tool_call_delta.emit(self.ctx, delta, begin)
+        self.tool_begin = True
 
     @override
     def on_tool_call_done(self, tool_call) -> None:
         """Callback that is fired when a tool call delta is encountered"""
         self.signals.stream_tool_call_done.emit(self.ctx, tool_call, self.tool_begin)
 
 
@@ -376,19 +487,21 @@
     finished = Signal(object, object, bool)  # ctx, run, stream
     error = Signal(object, object)  # ctx, error
 
     # stream
     stream_text_created = Signal(object)  # ctx
     stream_text_delta = Signal(object, object, bool)  # ctx, delta, begin
     stream_end = Signal(object)  # ctx
-    stream_tool_call_created = Signal(object, object)  # ctx, tool_call
-    stream_tool_call_delta = Signal(object, object, bool)  # ctx, delta
+    stream_tool_call_created = Signal(object, object, bool)  # ctx, tool_call, begin
+    stream_tool_call_delta = Signal(object, object, bool)  # ctx, delta, begin
     stream_tool_call_done = Signal(object, object, bool)  # ctx, tool_call
     stream_message_done = Signal(object, object)  # ctx, message
-    stream_run_step_created = Signal(object, object)  # ctx, run_step
+    stream_run_step_created = Signal(object, object, int)  # ctx, run_step, step idx
+    stream_run_created = Signal(object, object)  # ctx, run_step
+    stream_run_step_done = Signal(object, object, int)  # ctx, run_step, step idx
 
 
 class Worker(QRunnable):
     """Assistants worker"""
     def __init__(self, *args, **kwargs):
         super(Worker, self).__init__()
         self.signals = WorkerSignals()
```

### Comparing `pygpt_net-2.2.1/src/pygpt_net/provider/gpt/worker/importer.py` & `pygpt_net-2.2.2/src/pygpt_net/provider/gpt/worker/importer.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/provider/llms/anthropic.py` & `pygpt_net-2.2.2/src/pygpt_net/provider/llms/anthropic.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/provider/llms/azure_openai.py` & `pygpt_net-2.2.2/src/pygpt_net/provider/llms/azure_openai.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/provider/llms/base.py` & `pygpt_net-2.2.2/src/pygpt_net/provider/llms/base.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/provider/llms/hugging_face.py` & `pygpt_net-2.2.2/src/pygpt_net/provider/llms/hugging_face.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/provider/llms/llama.py` & `pygpt_net-2.2.2/src/pygpt_net/provider/llms/llama.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/provider/llms/ollama.py` & `pygpt_net-2.2.2/src/pygpt_net/provider/llms/ollama.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/provider/llms/openai.py` & `pygpt_net-2.2.2/src/pygpt_net/provider/llms/openai.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/provider/loaders/base.py` & `pygpt_net-2.2.2/src/pygpt_net/provider/loaders/base.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/provider/loaders/file_csv.py` & `pygpt_net-2.2.2/src/pygpt_net/provider/loaders/file_csv.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/provider/loaders/file_docx.py` & `pygpt_net-2.2.2/src/pygpt_net/provider/loaders/file_docx.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/provider/loaders/file_epub.py` & `pygpt_net-2.2.2/src/pygpt_net/provider/loaders/file_epub.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/provider/loaders/file_excel.py` & `pygpt_net-2.2.2/src/pygpt_net/provider/loaders/file_excel.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/provider/loaders/file_html.py` & `pygpt_net-2.2.2/src/pygpt_net/provider/loaders/file_html.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/provider/loaders/file_image_vision.py` & `pygpt_net-2.2.2/src/pygpt_net/provider/loaders/file_image_vision.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/provider/loaders/file_ipynb.py` & `pygpt_net-2.2.2/src/pygpt_net/provider/loaders/file_ipynb.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/provider/loaders/file_json.py` & `pygpt_net-2.2.2/src/pygpt_net/provider/loaders/file_json.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/provider/loaders/file_markdown.py` & `pygpt_net-2.2.2/src/pygpt_net/provider/loaders/file_markdown.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/provider/loaders/file_pdf.py` & `pygpt_net-2.2.2/src/pygpt_net/provider/loaders/file_pdf.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/provider/loaders/file_video_audio.py` & `pygpt_net-2.2.2/src/pygpt_net/provider/loaders/file_video_audio.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/provider/loaders/file_xml.py` & `pygpt_net-2.2.2/src/pygpt_net/provider/loaders/file_xml.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/provider/loaders/hub/bitbucket/repo.py` & `pygpt_net-2.2.2/src/pygpt_net/provider/loaders/hub/bitbucket/repo.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/provider/loaders/hub/chatgpt_retrieval/base.py` & `pygpt_net-2.2.2/src/pygpt_net/provider/loaders/hub/chatgpt_retrieval/base.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/provider/loaders/hub/database/base.py` & `pygpt_net-2.2.2/src/pygpt_net/provider/loaders/hub/database/base.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/provider/loaders/hub/github/issues.py` & `pygpt_net-2.2.2/src/pygpt_net/provider/loaders/hub/github/issues.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/provider/loaders/hub/github/repo.py` & `pygpt_net-2.2.2/src/pygpt_net/provider/loaders/hub/github/repo.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/provider/loaders/hub/google/calendar.py` & `pygpt_net-2.2.2/src/pygpt_net/provider/loaders/hub/google/calendar.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/provider/loaders/hub/google/docs.py` & `pygpt_net-2.2.2/src/pygpt_net/provider/loaders/hub/google/docs.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/provider/loaders/hub/google/gmail.py` & `pygpt_net-2.2.2/src/pygpt_net/provider/loaders/hub/google/gmail.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/provider/loaders/hub/google/keep.py` & `pygpt_net-2.2.2/src/pygpt_net/provider/loaders/hub/google/keep.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/provider/loaders/hub/google/sheets.py` & `pygpt_net-2.2.2/src/pygpt_net/provider/loaders/hub/google/sheets.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/provider/loaders/hub/image_vision/base.py` & `pygpt_net-2.2.2/src/pygpt_net/provider/loaders/hub/image_vision/base.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/provider/loaders/hub/json/base.py` & `pygpt_net-2.2.2/src/pygpt_net/provider/loaders/hub/json/base.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/provider/loaders/hub/pandas_excel/base.py` & `pygpt_net-2.2.2/src/pygpt_net/provider/loaders/hub/pandas_excel/base.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/provider/loaders/hub/simple_csv/base.py` & `pygpt_net-2.2.2/src/pygpt_net/provider/loaders/hub/simple_csv/base.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/provider/loaders/hub/video_audio/base.py` & `pygpt_net-2.2.2/src/pygpt_net/provider/loaders/hub/video_audio/base.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/provider/loaders/hub/web_page/base.py` & `pygpt_net-2.2.2/src/pygpt_net/provider/loaders/hub/web_page/base.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/provider/loaders/hub/yt/base.py` & `pygpt_net-2.2.2/src/pygpt_net/provider/loaders/hub/yt/base.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/provider/loaders/hub/yt/utils.py` & `pygpt_net-2.2.2/src/pygpt_net/provider/loaders/hub/yt/utils.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/provider/loaders/web_bitbucket.py` & `pygpt_net-2.2.2/src/pygpt_net/provider/loaders/web_bitbucket.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/provider/loaders/web_chatgpt_retrieval.py` & `pygpt_net-2.2.2/src/pygpt_net/provider/loaders/web_chatgpt_retrieval.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/provider/loaders/web_database.py` & `pygpt_net-2.2.2/src/pygpt_net/provider/loaders/web_database.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/provider/loaders/web_github_issues.py` & `pygpt_net-2.2.2/src/pygpt_net/provider/loaders/web_github_issues.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/provider/loaders/web_github_repo.py` & `pygpt_net-2.2.2/src/pygpt_net/provider/loaders/web_github_repo.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/provider/loaders/web_google_calendar.py` & `pygpt_net-2.2.2/src/pygpt_net/provider/loaders/web_google_calendar.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/provider/loaders/web_google_docs.py` & `pygpt_net-2.2.2/src/pygpt_net/provider/loaders/web_google_docs.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/provider/loaders/web_google_drive.py` & `pygpt_net-2.2.2/src/pygpt_net/provider/loaders/web_google_drive.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/provider/loaders/web_google_gmail.py` & `pygpt_net-2.2.2/src/pygpt_net/provider/loaders/web_google_gmail.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/provider/loaders/web_google_keep.py` & `pygpt_net-2.2.2/src/pygpt_net/provider/loaders/web_google_keep.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/provider/loaders/web_google_sheets.py` & `pygpt_net-2.2.2/src/pygpt_net/provider/loaders/web_google_sheets.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/provider/loaders/web_microsoft_onedrive.py` & `pygpt_net-2.2.2/src/pygpt_net/provider/loaders/web_microsoft_onedrive.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/provider/loaders/web_page.py` & `pygpt_net-2.2.2/src/pygpt_net/provider/loaders/web_page.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/provider/loaders/web_rss.py` & `pygpt_net-2.2.2/src/pygpt_net/provider/loaders/web_rss.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/provider/loaders/web_sitemap.py` & `pygpt_net-2.2.2/src/pygpt_net/provider/loaders/web_sitemap.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/provider/loaders/web_twitter.py` & `pygpt_net-2.2.2/src/pygpt_net/provider/loaders/web_twitter.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/provider/loaders/web_yt.py` & `pygpt_net-2.2.2/src/pygpt_net/provider/loaders/web_yt.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/provider/vector_stores/__init__.py` & `pygpt_net-2.2.2/src/pygpt_net/provider/vector_stores/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/provider/vector_stores/base.py` & `pygpt_net-2.2.2/src/pygpt_net/provider/vector_stores/base.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/provider/vector_stores/chroma.py` & `pygpt_net-2.2.2/src/pygpt_net/provider/vector_stores/chroma.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/provider/vector_stores/elasticsearch.py` & `pygpt_net-2.2.2/src/pygpt_net/provider/vector_stores/elasticsearch.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/provider/vector_stores/pinecode.py` & `pygpt_net-2.2.2/src/pygpt_net/provider/vector_stores/pinecode.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/provider/vector_stores/redis.py` & `pygpt_net-2.2.2/src/pygpt_net/provider/vector_stores/redis.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/provider/vector_stores/simple.py` & `pygpt_net-2.2.2/src/pygpt_net/provider/vector_stores/simple.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/provider/vector_stores/temp.py` & `pygpt_net-2.2.2/src/pygpt_net/provider/vector_stores/temp.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/provider/web/base.py` & `pygpt_net-2.2.2/src/pygpt_net/provider/web/base.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/provider/web/google_custom_search.py` & `pygpt_net-2.2.2/src/pygpt_net/provider/web/google_custom_search.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/provider/web/microsoft_bing.py` & `pygpt_net-2.2.2/src/pygpt_net/provider/web/microsoft_bing.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/tools/__init__.py` & `pygpt_net-2.2.2/src/pygpt_net/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/tools/audio_transcriber/__init__.py` & `pygpt_net-2.2.2/src/pygpt_net/tools/audio_transcriber/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/tools/audio_transcriber/ui/dialogs.py` & `pygpt_net-2.2.2/src/pygpt_net/tools/audio_transcriber/ui/dialogs.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/tools/base.py` & `pygpt_net-2.2.2/src/pygpt_net/tools/base.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/tools/code_interpreter/__init__.py` & `pygpt_net-2.2.2/src/pygpt_net/tools/code_interpreter/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/tools/code_interpreter/ui/dialogs.py` & `pygpt_net-2.2.2/src/pygpt_net/tools/code_interpreter/ui/dialogs.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/tools/code_interpreter/ui/widgets.py` & `pygpt_net-2.2.2/src/pygpt_net/tools/code_interpreter/ui/widgets.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/tools/image_viewer/__init__.py` & `pygpt_net-2.2.2/src/pygpt_net/tools/image_viewer/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/tools/image_viewer/ui/dialogs.py` & `pygpt_net-2.2.2/src/pygpt_net/tools/image_viewer/ui/dialogs.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/tools/indexer/__init__.py` & `pygpt_net-2.2.2/src/pygpt_net/tools/indexer/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/tools/indexer/ui/browse.py` & `pygpt_net-2.2.2/src/pygpt_net/tools/indexer/ui/browse.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/tools/indexer/ui/ctx.py` & `pygpt_net-2.2.2/src/pygpt_net/tools/indexer/ui/ctx.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/tools/indexer/ui/dialogs.py` & `pygpt_net-2.2.2/src/pygpt_net/tools/indexer/ui/dialogs.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/tools/indexer/ui/files.py` & `pygpt_net-2.2.2/src/pygpt_net/tools/indexer/ui/files.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/tools/indexer/ui/web.py` & `pygpt_net-2.2.2/src/pygpt_net/tools/indexer/ui/web.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/tools/indexer/ui/widgets.py` & `pygpt_net-2.2.2/src/pygpt_net/tools/indexer/ui/widgets.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/tools/media_player/__init__.py` & `pygpt_net-2.2.2/src/pygpt_net/tools/media_player/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/tools/media_player/ui/dialogs.py` & `pygpt_net-2.2.2/src/pygpt_net/tools/media_player/ui/dialogs.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/tools/media_player/ui/widgets.py` & `pygpt_net-2.2.2/src/pygpt_net/tools/media_player/ui/widgets.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/tools/text_editor/ui/dialogs.py` & `pygpt_net-2.2.2/src/pygpt_net/tools/text_editor/ui/dialogs.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/tools/text_editor/ui/widgets.py` & `pygpt_net-2.2.2/src/pygpt_net/tools/text_editor/ui/widgets.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/ui/__init__.py` & `pygpt_net-2.2.2/src/pygpt_net/ui/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/ui/base/config_dialog.py` & `pygpt_net-2.2.2/src/pygpt_net/ui/base/config_dialog.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/ui/base/context_menu.py` & `pygpt_net-2.2.2/src/pygpt_net/ui/base/context_menu.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/ui/dialog/about.py` & `pygpt_net-2.2.2/src/pygpt_net/ui/dialog/about.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/ui/dialog/applog.py` & `pygpt_net-2.2.2/src/pygpt_net/ui/dialog/applog.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/ui/dialog/assistant.py` & `pygpt_net-2.2.2/src/pygpt_net/ui/dialog/assistant.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/ui/dialog/assistant_store.py` & `pygpt_net-2.2.2/src/pygpt_net/ui/dialog/assistant_store.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/ui/dialog/changelog.py` & `pygpt_net-2.2.2/src/pygpt_net/ui/dialog/changelog.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/ui/dialog/create.py` & `pygpt_net-2.2.2/src/pygpt_net/ui/dialog/create.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/ui/dialog/db.py` & `pygpt_net-2.2.2/src/pygpt_net/ui/dialog/db.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/ui/dialog/debug.py` & `pygpt_net-2.2.2/src/pygpt_net/ui/dialog/debug.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/ui/dialog/dictionary.py` & `pygpt_net-2.2.2/src/pygpt_net/ui/dialog/dictionary.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/ui/dialog/editor.py` & `pygpt_net-2.2.2/src/pygpt_net/ui/dialog/editor.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/ui/dialog/find.py` & `pygpt_net-2.2.2/src/pygpt_net/ui/dialog/find.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/ui/dialog/image.py` & `pygpt_net-2.2.2/src/pygpt_net/ui/dialog/image.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/ui/dialog/license.py` & `pygpt_net-2.2.2/src/pygpt_net/ui/dialog/license.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/ui/dialog/logger.py` & `pygpt_net-2.2.2/src/pygpt_net/ui/dialog/logger.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/ui/dialog/models.py` & `pygpt_net-2.2.2/src/pygpt_net/ui/dialog/models.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/ui/dialog/plugins.py` & `pygpt_net-2.2.2/src/pygpt_net/ui/dialog/plugins.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/ui/dialog/preset.py` & `pygpt_net-2.2.2/src/pygpt_net/ui/dialog/preset.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/ui/dialog/preset_plugins.py` & `pygpt_net-2.2.2/src/pygpt_net/ui/dialog/preset_plugins.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/ui/dialog/profile.py` & `pygpt_net-2.2.2/src/pygpt_net/ui/dialog/profile.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/ui/dialog/rename.py` & `pygpt_net-2.2.2/src/pygpt_net/ui/dialog/rename.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/ui/dialog/settings.py` & `pygpt_net-2.2.2/src/pygpt_net/ui/dialog/settings.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/ui/dialog/snap.py` & `pygpt_net-2.2.2/src/pygpt_net/ui/dialog/snap.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/ui/dialog/start.py` & `pygpt_net-2.2.2/src/pygpt_net/ui/dialog/start.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/ui/dialog/update.py` & `pygpt_net-2.2.2/src/pygpt_net/ui/dialog/update.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/ui/dialog/workdir.py` & `pygpt_net-2.2.2/src/pygpt_net/ui/dialog/workdir.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/ui/dialogs.py` & `pygpt_net-2.2.2/src/pygpt_net/ui/dialogs.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/ui/layout/chat/__init__.py` & `pygpt_net-2.2.2/src/pygpt_net/ui/layout/chat/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/ui/layout/chat/attachments.py` & `pygpt_net-2.2.2/src/pygpt_net/ui/layout/chat/attachments.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/ui/layout/chat/attachments_uploaded.py` & `pygpt_net-2.2.2/src/pygpt_net/ui/layout/chat/attachments_uploaded.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/ui/layout/chat/calendar.py` & `pygpt_net-2.2.2/src/pygpt_net/ui/layout/chat/calendar.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/ui/layout/chat/input.py` & `pygpt_net-2.2.2/src/pygpt_net/ui/layout/chat/input.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/ui/layout/chat/markdown.py` & `pygpt_net-2.2.2/src/pygpt_net/ui/layout/chat/markdown.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/ui/layout/chat/output.py` & `pygpt_net-2.2.2/src/pygpt_net/ui/layout/chat/output.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/ui/layout/chat/painter.py` & `pygpt_net-2.2.2/src/pygpt_net/ui/layout/chat/painter.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/ui/layout/ctx/__init__.py` & `pygpt_net-2.2.2/src/pygpt_net/ui/layout/ctx/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/ui/layout/ctx/ctx_list.py` & `pygpt_net-2.2.2/src/pygpt_net/ui/layout/ctx/ctx_list.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/ui/layout/ctx/search_input.py` & `pygpt_net-2.2.2/src/pygpt_net/ui/layout/ctx/search_input.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/ui/layout/ctx/video.py` & `pygpt_net-2.2.2/src/pygpt_net/ui/layout/ctx/video.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/ui/layout/status.py` & `pygpt_net-2.2.2/src/pygpt_net/ui/layout/status.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/ui/layout/toolbox/__init__.py` & `pygpt_net-2.2.2/src/pygpt_net/ui/layout/toolbox/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/ui/layout/toolbox/agent.py` & `pygpt_net-2.2.2/src/pygpt_net/ui/layout/toolbox/agent.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/ui/layout/toolbox/assistants.py` & `pygpt_net-2.2.2/src/pygpt_net/ui/layout/toolbox/assistants.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/ui/layout/toolbox/footer.py` & `pygpt_net-2.2.2/src/pygpt_net/ui/layout/toolbox/footer.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/ui/layout/toolbox/image.py` & `pygpt_net-2.2.2/src/pygpt_net/ui/layout/toolbox/image.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/ui/layout/toolbox/indexes.py` & `pygpt_net-2.2.2/src/pygpt_net/ui/layout/toolbox/indexes.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/ui/layout/toolbox/mode.py` & `pygpt_net-2.2.2/src/pygpt_net/ui/layout/toolbox/mode.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/ui/layout/toolbox/model.py` & `pygpt_net-2.2.2/src/pygpt_net/ui/layout/toolbox/model.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/ui/layout/toolbox/presets.py` & `pygpt_net-2.2.2/src/pygpt_net/ui/layout/toolbox/presets.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/ui/layout/toolbox/prompt.py` & `pygpt_net-2.2.2/src/pygpt_net/ui/layout/toolbox/prompt.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/ui/layout/toolbox/vision.py` & `pygpt_net-2.2.2/src/pygpt_net/ui/layout/toolbox/vision.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/ui/main.py` & `pygpt_net-2.2.2/src/pygpt_net/ui/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # -*- coding: utf-8 -*-
 # ================================================== #
 # This file is a part of PYGPT package               #
 # Website: https://pygpt.net                         #
 # GitHub:  https://github.com/szczyglis-dev/py-gpt   #
 # MIT License                                        #
 # Created By  : Marcin Szczygliński                  #
-# Updated Date: 2024.04.20 22:00:00                  #
+# Updated Date: 2024.04.29 07:00:00                  #
 # ================================================== #
 
 import os
 
 from PySide6.QtCore import QTimer, Signal, Slot, QThreadPool, QEvent, Qt, QLoggingCategory
 from PySide6.QtWidgets import QApplication, QMainWindow
 from qt_material import QtStyleTools
@@ -59,14 +59,15 @@
         # load version info
         self.meta = get_app_meta()
 
         # setup service container
         self.core = Container(self)
         self.core.init()
         self.core.patch()  # patch version if needed
+        self.core.post_setup()
 
         # before render, handle engine args
         self.handle_engine_args()
 
         # setup thread pool
         self.threadpool = QThreadPool()
```

### Comparing `pygpt_net-2.2.1/src/pygpt_net/ui/menu/__init__.py` & `pygpt_net-2.2.2/src/pygpt_net/ui/menu/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/ui/menu/about.py` & `pygpt_net-2.2.2/src/pygpt_net/ui/menu/about.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/ui/menu/audio.py` & `pygpt_net-2.2.2/src/pygpt_net/ui/menu/audio.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/ui/menu/config.py` & `pygpt_net-2.2.2/src/pygpt_net/ui/menu/config.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/ui/menu/debug.py` & `pygpt_net-2.2.2/src/pygpt_net/ui/menu/debug.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/ui/menu/file.py` & `pygpt_net-2.2.2/src/pygpt_net/ui/menu/file.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/ui/menu/lang.py` & `pygpt_net-2.2.2/src/pygpt_net/ui/menu/lang.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/ui/menu/plugins.py` & `pygpt_net-2.2.2/src/pygpt_net/ui/menu/plugins.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/ui/menu/theme.py` & `pygpt_net-2.2.2/src/pygpt_net/ui/menu/theme.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/ui/menu/tools.py` & `pygpt_net-2.2.2/src/pygpt_net/ui/menu/tools.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/ui/menu/video.py` & `pygpt_net-2.2.2/src/pygpt_net/ui/menu/video.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/ui/tray.py` & `pygpt_net-2.2.2/src/pygpt_net/ui/tray.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/ui/widget/audio/input.py` & `pygpt_net-2.2.2/src/pygpt_net/ui/widget/audio/input.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/ui/widget/audio/input_button.py` & `pygpt_net-2.2.2/src/pygpt_net/ui/widget/audio/input_button.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/ui/widget/audio/output.py` & `pygpt_net-2.2.2/src/pygpt_net/ui/widget/audio/output.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/ui/widget/calendar/select.py` & `pygpt_net-2.2.2/src/pygpt_net/ui/widget/calendar/select.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/ui/widget/dialog/alert.py` & `pygpt_net-2.2.2/src/pygpt_net/ui/widget/dialog/alert.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/ui/widget/dialog/applog.py` & `pygpt_net-2.2.2/src/pygpt_net/ui/widget/dialog/applog.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/ui/widget/dialog/assistant_store.py` & `pygpt_net-2.2.2/src/pygpt_net/ui/widget/dialog/assistant_store.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/ui/widget/dialog/audio.py` & `pygpt_net-2.2.2/src/pygpt_net/ui/widget/dialog/audio.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/ui/widget/dialog/base.py` & `pygpt_net-2.2.2/src/pygpt_net/ui/widget/dialog/base.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/ui/widget/dialog/confirm.py` & `pygpt_net-2.2.2/src/pygpt_net/ui/widget/dialog/confirm.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/ui/widget/dialog/create.py` & `pygpt_net-2.2.2/src/pygpt_net/ui/widget/dialog/create.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/ui/widget/dialog/db.py` & `pygpt_net-2.2.2/src/pygpt_net/ui/widget/dialog/db.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/ui/widget/dialog/debug.py` & `pygpt_net-2.2.2/src/pygpt_net/ui/widget/dialog/debug.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/ui/widget/dialog/editor.py` & `pygpt_net-2.2.2/src/pygpt_net/ui/widget/dialog/editor.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/ui/widget/dialog/editor_file.py` & `pygpt_net-2.2.2/src/pygpt_net/ui/widget/dialog/editor_file.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/ui/widget/dialog/find.py` & `pygpt_net-2.2.2/src/pygpt_net/ui/widget/dialog/find.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/ui/widget/dialog/image.py` & `pygpt_net-2.2.2/src/pygpt_net/ui/widget/dialog/image.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/ui/widget/dialog/info.py` & `pygpt_net-2.2.2/src/pygpt_net/ui/widget/dialog/info.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/ui/widget/dialog/license.py` & `pygpt_net-2.2.2/src/pygpt_net/ui/widget/dialog/license.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/ui/widget/dialog/logger.py` & `pygpt_net-2.2.2/src/pygpt_net/ui/widget/dialog/logger.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/ui/widget/dialog/model.py` & `pygpt_net-2.2.2/src/pygpt_net/ui/widget/dialog/model.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/ui/widget/dialog/preset_plugins.py` & `pygpt_net-2.2.2/src/pygpt_net/ui/widget/dialog/preset_plugins.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/ui/widget/dialog/profile.py` & `pygpt_net-2.2.2/src/pygpt_net/ui/widget/dialog/profile.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/ui/widget/dialog/rename.py` & `pygpt_net-2.2.2/src/pygpt_net/ui/widget/dialog/rename.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/ui/widget/dialog/settings.py` & `pygpt_net-2.2.2/src/pygpt_net/ui/widget/dialog/settings.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/ui/widget/dialog/settings_plugin.py` & `pygpt_net-2.2.2/src/pygpt_net/ui/widget/dialog/settings_plugin.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/ui/widget/dialog/snap.py` & `pygpt_net-2.2.2/src/pygpt_net/ui/widget/dialog/snap.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/ui/widget/dialog/update.py` & `pygpt_net-2.2.2/src/pygpt_net/ui/widget/dialog/update.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/ui/widget/dialog/workdir.py` & `pygpt_net-2.2.2/src/pygpt_net/ui/widget/dialog/workdir.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/ui/widget/draw/painter.py` & `pygpt_net-2.2.2/src/pygpt_net/ui/widget/draw/painter.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/ui/widget/element/button.py` & `pygpt_net-2.2.2/src/pygpt_net/ui/widget/element/button.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/ui/widget/element/checkbox.py` & `pygpt_net-2.2.2/src/pygpt_net/ui/widget/element/checkbox.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/ui/widget/element/group.py` & `pygpt_net-2.2.2/src/pygpt_net/ui/widget/element/group.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/ui/widget/element/labels.py` & `pygpt_net-2.2.2/src/pygpt_net/ui/widget/element/labels.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/ui/widget/filesystem/explorer.py` & `pygpt_net-2.2.2/src/pygpt_net/ui/widget/filesystem/explorer.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/ui/widget/image/display.py` & `pygpt_net-2.2.2/src/pygpt_net/ui/widget/image/display.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/ui/widget/lists/assistant.py` & `pygpt_net-2.2.2/src/pygpt_net/ui/widget/lists/assistant.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/ui/widget/lists/assistant_store.py` & `pygpt_net-2.2.2/src/pygpt_net/ui/widget/lists/assistant_store.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/ui/widget/lists/attachment.py` & `pygpt_net-2.2.2/src/pygpt_net/ui/widget/lists/attachment.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/ui/widget/lists/base.py` & `pygpt_net-2.2.2/src/pygpt_net/ui/widget/lists/base.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/ui/widget/lists/context.py` & `pygpt_net-2.2.2/src/pygpt_net/ui/widget/lists/context.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/ui/widget/lists/db.py` & `pygpt_net-2.2.2/src/pygpt_net/ui/widget/lists/db.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/ui/widget/lists/debug.py` & `pygpt_net-2.2.2/src/pygpt_net/ui/widget/lists/debug.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/ui/widget/lists/index.py` & `pygpt_net-2.2.2/src/pygpt_net/ui/widget/lists/index.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/ui/widget/lists/index_combo.py` & `pygpt_net-2.2.2/src/pygpt_net/ui/widget/lists/index_combo.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/ui/widget/lists/mode.py` & `pygpt_net-2.2.2/src/pygpt_net/ui/widget/lists/mode.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/ui/widget/lists/model.py` & `pygpt_net-2.2.2/src/pygpt_net/ui/widget/lists/model.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/ui/widget/lists/model_editor.py` & `pygpt_net-2.2.2/src/pygpt_net/ui/widget/lists/model_editor.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/ui/widget/lists/plugin.py` & `pygpt_net-2.2.2/src/pygpt_net/ui/widget/lists/plugin.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/ui/widget/lists/preset.py` & `pygpt_net-2.2.2/src/pygpt_net/ui/widget/lists/preset.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/ui/widget/lists/preset_plugins.py` & `pygpt_net-2.2.2/src/pygpt_net/ui/widget/lists/preset_plugins.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/ui/widget/lists/profile.py` & `pygpt_net-2.2.2/src/pygpt_net/ui/widget/lists/profile.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/ui/widget/lists/settings.py` & `pygpt_net-2.2.2/src/pygpt_net/ui/widget/lists/settings.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/ui/widget/lists/uploaded.py` & `pygpt_net-2.2.2/src/pygpt_net/ui/widget/lists/uploaded.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/ui/widget/option/checkbox.py` & `pygpt_net-2.2.2/src/pygpt_net/ui/widget/option/checkbox.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/ui/widget/option/cmd.py` & `pygpt_net-2.2.2/src/pygpt_net/ui/widget/option/cmd.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/ui/widget/option/combo.py` & `pygpt_net-2.2.2/src/pygpt_net/ui/widget/option/combo.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/ui/widget/option/dictionary.py` & `pygpt_net-2.2.2/src/pygpt_net/ui/widget/option/dictionary.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/ui/widget/option/input.py` & `pygpt_net-2.2.2/src/pygpt_net/ui/widget/option/input.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/ui/widget/option/prompt.py` & `pygpt_net-2.2.2/src/pygpt_net/ui/widget/option/prompt.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/ui/widget/option/slider.py` & `pygpt_net-2.2.2/src/pygpt_net/ui/widget/option/slider.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/ui/widget/option/textarea.py` & `pygpt_net-2.2.2/src/pygpt_net/ui/widget/option/textarea.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/ui/widget/tabs/Input.py` & `pygpt_net-2.2.2/src/pygpt_net/ui/widget/tabs/Input.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/ui/widget/tabs/output.py` & `pygpt_net-2.2.2/src/pygpt_net/ui/widget/tabs/output.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/ui/widget/textarea/calendar_note.py` & `pygpt_net-2.2.2/src/pygpt_net/ui/widget/textarea/calendar_note.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/ui/widget/textarea/create.py` & `pygpt_net-2.2.2/src/pygpt_net/ui/widget/textarea/create.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/ui/widget/textarea/editor.py` & `pygpt_net-2.2.2/src/pygpt_net/ui/widget/textarea/editor.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/ui/widget/textarea/find.py` & `pygpt_net-2.2.2/src/pygpt_net/ui/widget/textarea/find.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/ui/widget/textarea/input.py` & `pygpt_net-2.2.2/src/pygpt_net/ui/widget/textarea/input.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/ui/widget/textarea/name.py` & `pygpt_net-2.2.2/src/pygpt_net/ui/widget/textarea/name.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/ui/widget/textarea/notepad.py` & `pygpt_net-2.2.2/src/pygpt_net/ui/widget/textarea/notepad.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/ui/widget/textarea/output.py` & `pygpt_net-2.2.2/src/pygpt_net/ui/widget/textarea/output.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/ui/widget/textarea/rename.py` & `pygpt_net-2.2.2/src/pygpt_net/ui/widget/textarea/rename.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/ui/widget/textarea/search_input.py` & `pygpt_net-2.2.2/src/pygpt_net/ui/widget/textarea/search_input.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/ui/widget/textarea/web.py` & `pygpt_net-2.2.2/src/pygpt_net/ui/widget/textarea/web.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/ui/widget/vision/camera.py` & `pygpt_net-2.2.2/src/pygpt_net/ui/widget/vision/camera.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/src/pygpt_net/utils.py` & `pygpt_net-2.2.2/src/pygpt_net/utils.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.1/PKG-INFO` & `pygpt_net-2.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygpt-net
-Version: 2.2.1
+Version: 2.2.2
 Summary: Desktop AI Assistant powered by GPT-4, GPT-4V, GPT-3.5, DALL-E 3, Langchain LLMs, Llama-index, Whisper with chatbot, assistant, text completion, vision and image generation, internet access, chat with files, commands and code execution, file upload and download and more
 Home-page: https://github.com/szczyglis-dev/py-gpt
 License: MIT
 Keywords: py_gpt,py-gpt,pygpt,desktop,app,gpt,gpt4,gpt4-v,gpt3.5,gpt-4,gpt-4V,gpt-3.5,tts,whisper,vision,chatgpt,dall-e,chat,chatbot,assistant,text completion,image generation,ai,api,openai,api key,langchain,llama-index,presets,ui,qt,pyside
 Author: Marcin Szczyglinski
 Author-email: info@pygpt.net
 Requires-Python: >=3.10,<3.12
@@ -70,15 +70,15 @@
 Project-URL: Repository, https://github.com/szczyglis-dev/py-gpt
 Description-Content-Type: text/markdown
 
 # PyGPT - Desktop AI Assistant
 
 [![pygpt](https://snapcraft.io/pygpt/badge.svg)](https://snapcraft.io/pygpt)
 
-Release: **2.2.1** | build: **2024.04.28** | Python: **>=3.10, <3.12**
+Release: **2.2.2** | build: **2024.04.29** | Python: **>=3.10, <3.12**
 
 Official website: https://pygpt.net | Documentation: https://pygpt.readthedocs.io
 
 Snap Store: https://snapcraft.io/pygpt | PyPi: https://pypi.org/project/pygpt-net
 
 Compiled version for Linux (`tar.gz`) and Windows 10/11 (`msi`) 64-bit: https://pygpt.net/#download
 
@@ -2739,14 +2739,16 @@
 
 - `Minimize to tray on exit`: Minimize to tray icon on exit. Tray icon enabled is required for this option to work. Default: False.
 
 - `Render engine`: chat output render engine: `WebEngine / Chromium` - for full HTML/CSS and `Legacy (markdown)` for legacy, simple markdown CSS output. Default: WebEngine / Chromium.
 
 - `OpenGL hardware acceleration`: enables hardware acceleration in `WebEngine / Chromium` renderer.  Default: False.
 
+- `Application environment (os.environ)`: Additional environment vars to set on application start.
+
 **Layout**
 
 - `Zoom`: Adjusts the zoom in chat window (web render view). `WebEngine / Chromium` render mode only.
 
 - `Code syntax highlight`: Syntax highlight theme in code blocks. `WebEngine / Chromium` render mode only.
 
 - `Font Size (chat window)`: Adjusts the font size in the chat window (plain-text) and notepads.
@@ -3124,14 +3126,22 @@
 
 ---
 
 # CHANGELOG
 
 ## Recent changes:
 
+**2.2.2 (2024-04-29)**
+
+- Added 'Application environment' option to Config -> General for setting up custom env vars on app load.
+- Added chunk render/parse throttling to prevent high CPU load on huge text chunks.
+- Optimized and improved Code interpreter output rendering in stream mode in Assistants.
+- Improved run stopping in Assistants.
+- Fixed syntax theme and 'Edit' icon restore on profile switch.
+
 **2.2.1 (2024-04-28)**
 
 - Improved data reload on profile switch.
 
 **2.2.0 (2024-04-28)**
 
 - Improved code interpreter stream handling in Assistant mode.
```

