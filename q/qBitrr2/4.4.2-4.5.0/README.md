# Comparing `tmp/qBitrr2-4.4.2.tar.gz` & `tmp/qbitrr2-4.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qBitrr2-4.4.2.tar", last modified: Tue Mar 26 08:50:57 2024, max compression
+gzip compressed data, was "qbitrr2-4.5.0.tar", last modified: Mon Apr 29 15:11:17 2024, max compression
```

## Comparing `qBitrr2-4.4.2.tar` & `qbitrr2-4.5.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 08:50:57.842948 qBitrr2-4.4.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-03-26 08:50:53.000000 qBitrr2-4.4.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    11089 2024-03-26 08:50:57.842948 qBitrr2-4.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8253 2024-03-26 08:50:53.000000 qBitrr2-4.4.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      805 2024-03-26 08:50:53.000000 qBitrr2-4.4.2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 08:50:57.838948 qBitrr2-4.4.2/qBitrr/
--rw-r--r--   0 runner    (1001) docker     (127)      405 2024-03-26 08:50:53.000000 qBitrr2-4.4.2/qBitrr/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)   221786 2024-03-26 08:50:53.000000 qBitrr2-4.4.2/qBitrr/arss.py
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-03-26 08:50:53.000000 qBitrr2-4.4.2/qBitrr/bundled_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     5259 2024-03-26 08:50:53.000000 qBitrr2-4.4.2/qBitrr/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2150 2024-03-26 08:50:53.000000 qBitrr2-4.4.2/qBitrr/env_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-03-26 08:50:53.000000 qBitrr2-4.4.2/qBitrr/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     4019 2024-03-26 08:50:53.000000 qBitrr2-4.4.2/qBitrr/ffprobe.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    26588 2024-03-26 08:50:53.000000 qBitrr2-4.4.2/qBitrr/gen_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      626 2024-03-26 08:50:53.000000 qBitrr2-4.4.2/qBitrr/home_path.py
--rw-r--r--   0 runner    (1001) docker     (127)     4478 2024-03-26 08:50:53.000000 qBitrr2-4.4.2/qBitrr/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     7347 2024-03-26 08:50:53.000000 qBitrr2-4.4.2/qBitrr/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     2187 2024-03-26 08:50:53.000000 qBitrr2-4.4.2/qBitrr/tables.py
--rw-r--r--   0 runner    (1001) docker     (127)     5849 2024-03-26 08:50:53.000000 qBitrr2-4.4.2/qBitrr/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 08:50:57.838948 qBitrr2-4.4.2/qBitrr2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11089 2024-03-26 08:50:57.000000 qBitrr2-4.4.2/qBitrr2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      475 2024-03-26 08:50:57.000000 qBitrr2-4.4.2/qBitrr2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-26 08:50:57.000000 qBitrr2-4.4.2/qBitrr2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-03-26 08:50:57.000000 qBitrr2-4.4.2/qBitrr2.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      614 2024-03-26 08:50:57.000000 qBitrr2-4.4.2/qBitrr2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-03-26 08:50:57.000000 qBitrr2-4.4.2/qBitrr2.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1942 2024-03-26 08:50:57.842948 qBitrr2-4.4.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-26 08:50:53.000000 qBitrr2-4.4.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:11:17.399261 qbitrr2-4.5.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-29 15:11:12.000000 qbitrr2-4.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    11089 2024-04-29 15:11:17.399261 qbitrr2-4.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8253 2024-04-29 15:11:12.000000 qbitrr2-4.5.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      805 2024-04-29 15:11:12.000000 qbitrr2-4.5.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:11:17.395261 qbitrr2-4.5.0/qBitrr/
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2024-04-29 15:11:12.000000 qbitrr2-4.5.0/qBitrr/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)   226578 2024-04-29 15:11:12.000000 qbitrr2-4.5.0/qBitrr/arss.py
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-04-29 15:11:12.000000 qbitrr2-4.5.0/qBitrr/bundled_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5259 2024-04-29 15:11:12.000000 qbitrr2-4.5.0/qBitrr/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2150 2024-04-29 15:11:12.000000 qbitrr2-4.5.0/qBitrr/env_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-04-29 15:11:12.000000 qbitrr2-4.5.0/qBitrr/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4019 2024-04-29 15:11:12.000000 qbitrr2-4.5.0/qBitrr/ffprobe.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    26588 2024-04-29 15:11:12.000000 qbitrr2-4.5.0/qBitrr/gen_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      626 2024-04-29 15:11:12.000000 qbitrr2-4.5.0/qBitrr/home_path.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4478 2024-04-29 15:11:12.000000 qbitrr2-4.5.0/qBitrr/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7347 2024-04-29 15:11:12.000000 qbitrr2-4.5.0/qBitrr/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2187 2024-04-29 15:11:12.000000 qbitrr2-4.5.0/qBitrr/tables.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5849 2024-04-29 15:11:12.000000 qbitrr2-4.5.0/qBitrr/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:11:17.399261 qbitrr2-4.5.0/qBitrr2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11089 2024-04-29 15:11:17.000000 qbitrr2-4.5.0/qBitrr2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-04-29 15:11:17.000000 qbitrr2-4.5.0/qBitrr2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 15:11:17.000000 qbitrr2-4.5.0/qBitrr2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-29 15:11:17.000000 qbitrr2-4.5.0/qBitrr2.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-04-29 15:11:17.000000 qbitrr2-4.5.0/qBitrr2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-29 15:11:17.000000 qbitrr2-4.5.0/qBitrr2.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1942 2024-04-29 15:11:17.403261 qbitrr2-4.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 15:11:12.000000 qbitrr2-4.5.0/setup.py
```

### Comparing `qBitrr2-4.4.2/LICENSE` & `qbitrr2-4.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `qBitrr2-4.4.2/PKG-INFO` & `qbitrr2-4.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qBitrr2
-Version: 4.4.2
+Version: 4.5.0
 Summary: "A simple Python script to talk to qBittorrent and Arr's"
 Home-page: https://github.com/Feramance/qBitrr
 Author: Feramance
 Author-email: fera@fera.wtf
 License: MIT
 Project-URL: Issue Tracker, https://github.com/Feramance/qBitrr/issues
 Project-URL: Source Code, https://github.com/Feramance/qBitrr
@@ -30,37 +30,37 @@
 License-File: LICENSE
 Requires-Dist: cachetools==5.3.2
 Requires-Dist: colorama==0.4.4
 Requires-Dist: coloredlogs==15.0.1
 Requires-Dist: environ-config==23.2.0
 Requires-Dist: ffmpeg-python==0.2.0
 Requires-Dist: jaraco.docker==2.0
-Requires-Dist: packaging==21.3
+Requires-Dist: packaging==22.0
 Requires-Dist: pathos==0.2.8
 Requires-Dist: peewee==3.14.7
 Requires-Dist: ping3==3.0.2
 Requires-Dist: pyarr==5.2.0
 Requires-Dist: qbittorrent-api==2023.7.52
 Requires-Dist: requests==2.31.0
 Requires-Dist: tomlkit==0.7.2
 Provides-Extra: dev
-Requires-Dist: black==22.1.0; extra == "dev"
+Requires-Dist: black==24.3.0; extra == "dev"
 Requires-Dist: bump2version==1.0.1; extra == "dev"
 Requires-Dist: isort==5.10.1; extra == "dev"
 Requires-Dist: pip-tools==7.3.0; extra == "dev"
 Requires-Dist: pre-commit==3.3.3; extra == "dev"
 Requires-Dist: pyinstaller==5.13.1; extra == "dev"
 Requires-Dist: pyupgrade==2.31.0; extra == "dev"
 Requires-Dist: twine==3.7.1; extra == "dev"
 Requires-Dist: ujson==5.4.0; extra == "dev"
 Requires-Dist: upgrade-pip==0.1.4; extra == "dev"
 Provides-Extra: fast
 Requires-Dist: ujson==5.4.0; extra == "fast"
 Provides-Extra: all
-Requires-Dist: black==22.1.0; extra == "all"
+Requires-Dist: black==24.3.0; extra == "all"
 Requires-Dist: bump2version==1.0.1; extra == "all"
 Requires-Dist: isort==5.10.1; extra == "all"
 Requires-Dist: pip-tools==7.3.0; extra == "all"
 Requires-Dist: pre-commit==3.3.3; extra == "all"
 Requires-Dist: pyinstaller==5.13.1; extra == "all"
 Requires-Dist: pyupgrade==2.31.0; extra == "all"
 Requires-Dist: twine==3.7.1; extra == "all"
```

### Comparing `qBitrr2-4.4.2/README.md` & `qbitrr2-4.5.0/README.md`

 * *Files identical despite different names*

### Comparing `qBitrr2-4.4.2/pyproject.toml` & `qbitrr2-4.5.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 
 [tool.black]
 line-length = 99
 target-version = ['py38']
 
 [tool.poetry]
 name = "pypi-public"
-version = "4.4.2"
+version = "4.5.0"
 description = "A simple script to monitor qBit and communicate with Radarr and Sonarr"
 authors = ["Drapersniper", "Feramance"]
 readme = "README.md"
 repository = "https://github.com/Feramance/qBitrr"
 url = "https://pypi.org/simple/"
 
 [tool.autopep8]
```

### Comparing `qBitrr2-4.4.2/qBitrr/arss.py` & `qbitrr2-4.5.0/qBitrr/arss.py`

 * *Files 2% similar despite different names*

```diff
@@ -114,20 +114,14 @@
                 self.completed_folder.chmod(mode=0o777)
             except BaseException:
                 self.logger.warning(
                     "%s completed folder is a soft requirement. The specified folder does not exist %s and cannot be created. This will disable all file monitoring.",
                     self._name,
                     self.completed_folder,
                 )
-        self.min_free_space = FREE_SPACE
-        if self.min_free_space != "-1":
-            self.current_free_space = shutil.disk_usage(self.completed_folder).free - parse_size(
-                self.min_free_space
-            )
-            self.logger.trace("Current free space: %s", self.current_free_space)
         self.apikey = CONFIG.get_or_raise(f"{name}.APIKey")
         self.re_search = CONFIG.get(f"{name}.ReSearch", fallback=False)
         self.import_mode = CONFIG.get(f"{name}.importMode", fallback="Auto")
         if self.import_mode == "Hardlink":
             self.import_mode = "Auto"
         self.refresh_downloads_timer = CONFIG.get(f"{name}.RefreshDownloadsTimer", fallback=1)
         self.arr_error_codes_to_blocklist = CONFIG.get(
@@ -484,15 +478,14 @@
                 else:
                     self.search_api_command = "MissingEpisodeSearch"
 
         self.manager.qbit_manager.client.torrents_create_tags(
             [
                 "qBitrr-allowed_seeding",
                 "qBitrr-ignored",
-                "qBitrr-free_space_paused",
                 "qbitrr-imported",
             ]
         )
         self.search_setup_completed = False
         self.model_file: EpisodeFilesModel | MoviesFilesModel = None
         self.series_file_model: SeriesFilesModel = None
         self.model_queue: EpisodeQueueModel | MovieQueueModel = None
@@ -2958,23 +2951,15 @@
                 if has_internet() is False:
                     self.manager.qbit_manager.should_delay_torrent_scan = True
                     raise DelayLoopException(length=NO_INTERNET_SLEEP_TIMER, type="internet")
                 if self.manager.qbit_manager.should_delay_torrent_scan:
                     raise DelayLoopException(length=NO_INTERNET_SLEEP_TIMER, type="delay")
                 self.api_calls()
                 self.refresh_download_queue()
-                if self.min_free_space != "-1":
-                    self.current_free_space = shutil.disk_usage(
-                        self.completed_folder
-                    ).free - parse_size(self.min_free_space)
-                    self.logger.trace("Current free space: %s", self.current_free_space)
-                    sorted_torrents = sorted(torrents, key=lambda t: t["priority"])
-                else:
-                    sorted_torrents = torrents
-                for torrent in sorted_torrents:
+                for torrent in torrents:
                     with contextlib.suppress(qbittorrentapi.NotFound404Error):
                         self._process_single_torrent(torrent)
                 self.process()
             except NoConnectionrException as e:
                 self.logger.error(e.message)
             except requests.exceptions.ConnectionError:
                 self.logger.warning("Couldn't connect to %s", self.type)
@@ -3323,32 +3308,14 @@
             torrent.state_enum,
             torrent.name,
             torrent.hash,
         )
         # We do not want to blacklist these!!
         self.remove_from_qbit.add(torrent.hash)
 
-    def _process_single_torrent_pause_disk_space(self, torrent: qbittorrentapi.TorrentDictionary):
-        self.logger.info(
-            "Pausing torrent for disk space: "
-            "[Progress: %s%%][Added On: %s]"
-            "[Availability: %s%%][Time Left: %s]"
-            "[Last active: %s] "
-            "| [%s] | %s (%s)",
-            round(torrent.progress * 100, 2),
-            datetime.fromtimestamp(self.recently_queue.get(torrent.hash, torrent.added_on)),
-            round(torrent.availability * 100, 2),
-            timedelta(seconds=torrent.eta),
-            datetime.fromtimestamp(torrent.last_activity),
-            torrent.state_enum,
-            torrent.name,
-            torrent.hash,
-        )
-        self.pause.add(torrent.hash)
-
     def _process_single_torrent_uploading(
         self, torrent: qbittorrentapi.TorrentDictionary, leave_alone: bool
     ):
         if leave_alone or torrent.state_enum == TorrentStates.FORCED_UPLOAD:
             self.logger.trace(
                 "Torrent State: Queued Upload | Allowing Seeding | "
                 "[Progress: %s%%][Added On: %s]"
@@ -3696,41 +3663,14 @@
         ratio_limit_tor = data_torrent.get("ratio_limit", -5)
         seeding_time_limit_dat = data_settings.get("seeding_time_limit", -5)
         seeding_time_limit_tor = data_torrent.get("seeding_time_limit", -5)
 
         seeding_time_limit = max(seeding_time_limit_dat, seeding_time_limit_tor)
         ratio_limit = max(ratio_limit_dat, ratio_limit_tor)
 
-        if self.is_downloading_state(torrent) and self.min_free_space != "-1":
-            free_space_test = self.current_free_space
-            free_space_test -= torrent["amount_left"]
-            self.logger.trace("Resulting free space: %s", free_space_test)
-            if (
-                torrent.state_enum != TorrentStates.PAUSED_DOWNLOAD
-                and self.current_free_space < torrent["amount_left"]
-            ):
-                self.logger.trace("Pause download: Free space %s", self.current_free_space)
-                torrent.add_tags(tags=["qBitrr-free_space_paused"])
-                torrent.remove_tags(tags=["qBitrr-allowed_seeding"])
-            elif (
-                torrent.state_enum == TorrentStates.PAUSED_DOWNLOAD
-                and self.current_free_space > torrent["amount_left"]
-            ):
-                self.current_free_space = free_space_test
-                self.logger.trace("Can download: Free space %s", self.current_free_space)
-                torrent.remove_tags(tags=["qBitrr-free_space_paused"])
-        elif self.is_complete_state(torrent) and "qBitrr-free_space_paused" in torrent.tags:
-            self.logger.trace(
-                "Removing tag[%s] for completed torrent[%s]: Free space %s",
-                "qBitrr-free_space_paused",
-                torrent,
-                self.current_free_space,
-            )
-            torrent.remove_tags(tags=["qBitrr-free_space_paused"])
-
         if self.seeding_mode_global_remove_torrent != -1 and self.remove_torrent(
             torrent, seeding_time_limit, ratio_limit
         ):
             remove_torrent = True
             return_value = False
         else:
             if torrent.ratio >= ratio_limit and ratio_limit != -5:
@@ -3924,20 +3864,15 @@
         if "qBitrr-ignored" in torrent.tags:
             torrent.remove_tags(
                 [
                     "qBitrr-allowed_seeding",
                     "qBitrr-free_space_paused",
                 ]
             )
-        if (
-            "qBitrr-free_space_paused" in torrent.tags
-            and torrent.state_enum != TorrentStates.PAUSED_DOWNLOAD
-        ):
-            self._process_single_torrent_pause_disk_space(torrent)
-        elif self.custom_format_unmet_search and self.custom_format_unmet_check(torrent):
+        if self.custom_format_unmet_search and self.custom_format_unmet_check(torrent):
             self._process_single_torrent_delete_cfunmet(torrent)
         elif remove_torrent and not leave_alone and torrent.amount_left == 0:
             self._process_single_torrent_delete_ratio_seed(torrent)
         elif torrent.category == FAILED_CATEGORY:
             # Bypass everything if manually marked as failed
             self._process_single_torrent_failed_cat(torrent)
         elif torrent.category == RECHECK_CATEGORY:
@@ -4047,16 +3982,14 @@
                     return
                 # A downloading torrent is not stalled, parse its contents.
                 self._process_single_torrent_process_files(torrent)
         elif self.is_complete_state(torrent) and leave_alone:
             self._process_single_completed_paused_torrent(torrent, leave_alone)
         else:
             self._process_single_torrent_unprocessed(torrent)
-        if "qBitrr-free_space_paused" in torrent.tags:
-            self._process_single_torrent_pause_disk_space(torrent)
 
     def custom_format_unmet_check(self, torrent: qbittorrentapi.TorrentDictionary) -> bool:
         try:
             completed = True
             while completed:
                 completed = False
                 try:
@@ -4228,23 +4161,17 @@
                 self.requeue_cache = {
                     entry["id"]: entry["movieId"] for entry in self.queue if entry.get("movieId")
                 }
                 self.queue_file_ids = {
                     entry["movieId"] for entry in self.queue if entry.get("movieId")
                 }
                 if self.model_queue:
-                    queue_before = self.model_queue.select(self.model_queue.EntryId).execute()
-                    {entry for entry in queue_before if entry}
-                    self.logger.debug("Queue before: %s", queue_before)
                     self.model_queue.delete().where(
                         self.model_queue.EntryId.not_in(list(self.queue_file_ids))
                     ).execute()
-                    queue_after = self.model_queue.select(self.model_queue.EntryId).execute()
-                    {entry for entry in queue_before if entry}
-                    self.logger.debug("Queue after: %s", queue_after)
 
         self._update_bad_queue_items()
 
     def get_queue(
         self,
         page=1,
         page_size=1000,
@@ -4754,15 +4681,27 @@
         self.ignore_torrents_younger_than = CONFIG.get(
             "Settings.IgnoreTorrentsYoungerThan", fallback=600
         )
         self.timed_ignore_cache = ExpiringSet(max_age_seconds=self.ignore_torrents_younger_than)
         self.timed_skip = ExpiringSet(max_age_seconds=self.ignore_torrents_younger_than)
         self.tracker_delay = ExpiringSet(max_age_seconds=600)
         self._LOG_LEVEL = self.manager.qbit_manager.logger.level
-        self.logger = logging.getLogger(f"qBitrr.{self._name}")
+        if ENABLE_LOGS:
+            LOGS_FOLDER = HOME_PATH.joinpath("logs")
+            LOGS_FOLDER.mkdir(parents=True, exist_ok=True)
+            LOGS_FOLDER.chmod(mode=0o777)
+            logfile = LOGS_FOLDER.joinpath(self._name + ".log")
+            if pathlib.Path(logfile).is_file():
+                logold = LOGS_FOLDER.joinpath(self._name + ".log.old")
+                logfile.rename(logold)
+            fh = logging.FileHandler(logfile)
+            self.logger = logging.getLogger(f"qBitrr.{self._name}")
+            self.logger.addHandler(fh)
+        else:
+            self.logger = logging.getLogger(f"qBitrr.{self._name}")
         run_logs(self.logger)
         self.search_missing = False
         self.session = None
         self.logger.hnotice("Starting %s monitor", self._name)
 
     def _process_errored(self):
         # Recheck all torrents marked for rechecking.
@@ -4873,19 +4812,188 @@
         except DelayLoopException:
             raise
 
     def run_search_loop(self):
         return
 
 
+class FreeSpaceManager(Arr):
+    def __init__(self, categories: set[str], manager: ArrManager):
+        self._name = "FreeSpaceManager"
+        self.categories = categories
+        self.manager = manager
+        self.pause = set()
+        self.resume = set()
+        self.expiring_bool = ExpiringSet(max_age_seconds=10)
+        self._LOG_LEVEL = self.manager.qbit_manager.logger.level
+        if ENABLE_LOGS:
+            LOGS_FOLDER = HOME_PATH.joinpath("logs")
+            LOGS_FOLDER.mkdir(parents=True, exist_ok=True)
+            LOGS_FOLDER.chmod(mode=0o777)
+            logfile = LOGS_FOLDER.joinpath(self._name + ".log")
+            if pathlib.Path(logfile).is_file():
+                logold = LOGS_FOLDER.joinpath(self._name + ".log.old")
+                logfile.rename(logold)
+            fh = logging.FileHandler(logfile)
+            self.logger = logging.getLogger(f"qBitrr.{self._name}")
+            self.logger.addHandler(fh)
+        else:
+            self.logger = logging.getLogger(f"qBitrr.{self._name}")
+        run_logs(self.logger)
+        self.completed_folder = pathlib.Path(COMPLETED_DOWNLOAD_FOLDER)
+        self.min_free_space = FREE_SPACE
+        self.current_free_space = shutil.disk_usage(self.completed_folder).free - parse_size(
+            self.min_free_space
+        )
+        self.logger.trace("Current free space: %s", self.current_free_space)
+        self.manager.qbit_manager.client.torrents_create_tags(
+            [
+                "qBitrr-free_space_paused",
+            ]
+        )
+        self.search_missing = False
+        self.session = None
+        self.logger.hnotice("Starting %s monitor", self._name)
+
+    def _process_single_torrent_pause_disk_space(self, torrent: qbittorrentapi.TorrentDictionary):
+        self.logger.info(
+            "Pausing torrent for disk space: "
+            "[Progress: %s%%][Added On: %s]"
+            "[Availability: %s%%][Time Left: %s]"
+            "[Last active: %s] "
+            "| [%s] | %s (%s)",
+            round(torrent.progress * 100, 2),
+            datetime.fromtimestamp(torrent.added_on),
+            round(torrent.availability * 100, 2),
+            timedelta(seconds=torrent.eta),
+            datetime.fromtimestamp(torrent.last_activity),
+            torrent.state_enum,
+            torrent.name,
+            torrent.hash,
+        )
+        self.pause.add(torrent.hash)
+
+    def _process_single_torrent_resume_disk_space(self, torrent: qbittorrentapi.TorrentDictionary):
+        self.logger.info(
+            "Resuming torrent for disk space: "
+            "[Progress: %s%%][Added On: %s]"
+            "[Availability: %s%%][Time Left: %s]"
+            "[Last active: %s] "
+            "| [%s] | %s (%s)",
+            round(torrent.progress * 100, 2),
+            datetime.fromtimestamp(torrent.added_on),
+            round(torrent.availability * 100, 2),
+            timedelta(seconds=torrent.eta),
+            datetime.fromtimestamp(torrent.last_activity),
+            torrent.state_enum,
+            torrent.name,
+            torrent.hash,
+        )
+        self.resume.add(torrent.hash)
+
+    def _process_single_torrent(self, torrent):
+        if self.is_downloading_state(torrent):
+            free_space_test = self.current_free_space
+            free_space_test -= torrent["amount_left"]
+            self.logger.trace("Resulting free space: %s", free_space_test)
+            if (
+                torrent.state_enum != TorrentStates.PAUSED_DOWNLOAD
+                and self.current_free_space < torrent["amount_left"]
+            ):
+                self.logger.trace("Pause download: Free space %s", self.current_free_space)
+                torrent.add_tags(tags=["qBitrr-free_space_paused"])
+                torrent.remove_tags(tags=["qBitrr-allowed_seeding"])
+                self._process_single_torrent_pause_disk_space(torrent.hash)
+            elif (
+                torrent.state_enum == TorrentStates.PAUSED_DOWNLOAD
+                and self.current_free_space > torrent["amount_left"]
+            ):
+                self.current_free_space = free_space_test
+                self.logger.trace("Can download: Free space %s", self.current_free_space)
+                torrent.remove_tags(tags=["qBitrr-free_space_paused"])
+                self._process_single_torrent_resume_disk_space(torrent.hash)
+        elif self.is_complete_state(torrent) and "qBitrr-free_space_paused" in torrent.tags:
+            self.logger.trace(
+                "Removing tag[%s] for completed torrent[%s]: Free space %s",
+                "qBitrr-free_space_paused",
+                torrent,
+                self.current_free_space,
+            )
+            torrent.remove_tags(tags=["qBitrr-free_space_paused"])
+
+    def process(self):
+        self._process_paused()
+        self._process_resume()
+
+    def process_torrents(self):
+        try:
+            try:
+                completed = True
+                while completed:
+                    try:
+                        completed = False
+                        torrents = self.manager.qbit_manager.client.torrents.info(
+                            status_filter="all",
+                            sort="added_on",
+                            reverse=False,
+                        )
+                    except qbittorrentapi.exceptions.APIError:
+                        completed = True
+                torrents = [t for t in torrents if hasattr(t, "category")]
+                torrents = [t for t in torrents if t.category in self.categories]
+                if not len(torrents):
+                    raise DelayLoopException(length=5, type="no_downloads")
+                if has_internet() is False:
+                    self.manager.qbit_manager.should_delay_torrent_scan = True
+                    raise DelayLoopException(length=NO_INTERNET_SLEEP_TIMER, type="internet")
+                if self.manager.qbit_manager.should_delay_torrent_scan:
+                    raise DelayLoopException(length=NO_INTERNET_SLEEP_TIMER, type="delay")
+                self.current_free_space = shutil.disk_usage(
+                    self.completed_folder
+                ).free - parse_size(self.min_free_space)
+                self.logger.trace("Current free space: %s", self.current_free_space)
+                sorted_torrents = sorted(torrents, key=lambda t: t["priority"])
+                for torrent in sorted_torrents:
+                    with contextlib.suppress(qbittorrentapi.NotFound404Error):
+                        self._process_single_torrent(torrent)
+                if len(self.pause) == 0:
+                    self.logger.trace("No torrents to pause")
+                self.process()
+            except NoConnectionrException as e:
+                self.logger.error(e.message)
+            except qbittorrentapi.exceptions.APIError as e:
+                self.logger.error("The qBittorrent API returned an unexpected error")
+                self.logger.debug("Unexpected APIError from qBitTorrent", exc_info=e)
+                raise DelayLoopException(length=300, type="qbit")
+            except qbittorrentapi.exceptions.APIConnectionError as e:
+                self.logger.warning("Max retries exceeded")
+                raise DelayLoopException(length=300, type="qbit")
+            except DelayLoopException:
+                raise
+            except KeyboardInterrupt:
+                self.logger.hnotice("Detected Ctrl+C - Terminating process")
+                sys.exit(0)
+            except Exception as e:
+                self.logger.error(e, exc_info=sys.exc_info())
+        except KeyboardInterrupt:
+            self.logger.hnotice("Detected Ctrl+C - Terminating process")
+            sys.exit(0)
+        except DelayLoopException:
+            raise
+
+    def run_search_loop(self):
+        return
+
+
 class ArrManager:
     def __init__(self, qbitmanager: qBitManager):
         self.groups: set[str] = set()
         self.uris: set[str] = set()
         self.special_categories: set[str] = {FAILED_CATEGORY, RECHECK_CATEGORY}
+        self.arr_categories: set[str] = set()
         self.category_allowlist: set[str] = self.special_categories.copy()
         self.completed_folders: set[pathlib.Path] = set()
         self.managed_objects: dict[str, Arr] = {}
         self.qbit: qbittorrentapi.Client = qbitmanager.client
         self.qbit_manager: qBitManager = qbitmanager
         self.ffprobe_available: bool = self.qbit_manager.ffprobe_downloader.probe_path.exists()
         self.logger = logging.getLogger(
@@ -4912,19 +5020,23 @@
                 else:
                     call_cls = None
                 try:
                     managed_object = Arr(name, self, client_cls=call_cls)
                     self.groups.add(name)
                     self.uris.add(managed_object.uri)
                     self.managed_objects[managed_object.category] = managed_object
+                    self.arr_categories.add(managed_object.category)
                 except KeyError as e:
                     self.logger.critical(e)
                 except ValueError as e:
                     self.logger.exception(e)
                 except SkipException:
                     continue
                 except (OSError, TypeError) as e:
                     self.logger.exception(e)
+        if FREE_SPACE != "-1":
+            managed_object = FreeSpaceManager(self.arr_categories, self)
+            self.managed_objects["FreeSpaceManager"] = managed_object
         for cat in self.special_categories:
             managed_object = PlaceHolderArr(cat, self)
             self.managed_objects[cat] = managed_object
         return self
```

### Comparing `qBitrr2-4.4.2/qBitrr/config.py` & `qbitrr2-4.5.0/qBitrr/config.py`

 * *Files identical despite different names*

### Comparing `qBitrr2-4.4.2/qBitrr/env_config.py` & `qbitrr2-4.5.0/qBitrr/env_config.py`

 * *Files identical despite different names*

### Comparing `qBitrr2-4.4.2/qBitrr/errors.py` & `qbitrr2-4.5.0/qBitrr/errors.py`

 * *Files identical despite different names*

### Comparing `qBitrr2-4.4.2/qBitrr/ffprobe.py` & `qbitrr2-4.5.0/qBitrr/ffprobe.py`

 * *Files identical despite different names*

### Comparing `qBitrr2-4.4.2/qBitrr/gen_config.py` & `qbitrr2-4.5.0/qBitrr/gen_config.py`

 * *Files identical despite different names*

### Comparing `qBitrr2-4.4.2/qBitrr/home_path.py` & `qbitrr2-4.5.0/qBitrr/home_path.py`

 * *Files identical despite different names*

### Comparing `qBitrr2-4.4.2/qBitrr/logger.py` & `qbitrr2-4.5.0/qBitrr/logger.py`

 * *Files identical despite different names*

### Comparing `qBitrr2-4.4.2/qBitrr/main.py` & `qbitrr2-4.5.0/qBitrr/main.py`

 * *Files identical despite different names*

### Comparing `qBitrr2-4.4.2/qBitrr/tables.py` & `qbitrr2-4.5.0/qBitrr/tables.py`

 * *Files identical despite different names*

### Comparing `qBitrr2-4.4.2/qBitrr/utils.py` & `qbitrr2-4.5.0/qBitrr/utils.py`

 * *Files identical despite different names*

### Comparing `qBitrr2-4.4.2/qBitrr2.egg-info/PKG-INFO` & `qbitrr2-4.5.0/qBitrr2.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qBitrr2
-Version: 4.4.2
+Version: 4.5.0
 Summary: "A simple Python script to talk to qBittorrent and Arr's"
 Home-page: https://github.com/Feramance/qBitrr
 Author: Feramance
 Author-email: fera@fera.wtf
 License: MIT
 Project-URL: Issue Tracker, https://github.com/Feramance/qBitrr/issues
 Project-URL: Source Code, https://github.com/Feramance/qBitrr
@@ -30,37 +30,37 @@
 License-File: LICENSE
 Requires-Dist: cachetools==5.3.2
 Requires-Dist: colorama==0.4.4
 Requires-Dist: coloredlogs==15.0.1
 Requires-Dist: environ-config==23.2.0
 Requires-Dist: ffmpeg-python==0.2.0
 Requires-Dist: jaraco.docker==2.0
-Requires-Dist: packaging==21.3
+Requires-Dist: packaging==22.0
 Requires-Dist: pathos==0.2.8
 Requires-Dist: peewee==3.14.7
 Requires-Dist: ping3==3.0.2
 Requires-Dist: pyarr==5.2.0
 Requires-Dist: qbittorrent-api==2023.7.52
 Requires-Dist: requests==2.31.0
 Requires-Dist: tomlkit==0.7.2
 Provides-Extra: dev
-Requires-Dist: black==22.1.0; extra == "dev"
+Requires-Dist: black==24.3.0; extra == "dev"
 Requires-Dist: bump2version==1.0.1; extra == "dev"
 Requires-Dist: isort==5.10.1; extra == "dev"
 Requires-Dist: pip-tools==7.3.0; extra == "dev"
 Requires-Dist: pre-commit==3.3.3; extra == "dev"
 Requires-Dist: pyinstaller==5.13.1; extra == "dev"
 Requires-Dist: pyupgrade==2.31.0; extra == "dev"
 Requires-Dist: twine==3.7.1; extra == "dev"
 Requires-Dist: ujson==5.4.0; extra == "dev"
 Requires-Dist: upgrade-pip==0.1.4; extra == "dev"
 Provides-Extra: fast
 Requires-Dist: ujson==5.4.0; extra == "fast"
 Provides-Extra: all
-Requires-Dist: black==22.1.0; extra == "all"
+Requires-Dist: black==24.3.0; extra == "all"
 Requires-Dist: bump2version==1.0.1; extra == "all"
 Requires-Dist: isort==5.10.1; extra == "all"
 Requires-Dist: pip-tools==7.3.0; extra == "all"
 Requires-Dist: pre-commit==3.3.3; extra == "all"
 Requires-Dist: pyinstaller==5.13.1; extra == "all"
 Requires-Dist: pyupgrade==2.31.0; extra == "all"
 Requires-Dist: twine==3.7.1; extra == "all"
```

### Comparing `qBitrr2-4.4.2/qBitrr2.egg-info/requires.txt` & `qbitrr2-4.5.0/qBitrr2.egg-info/requires.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 cachetools==5.3.2
 colorama==0.4.4
 coloredlogs==15.0.1
 environ-config==23.2.0
 ffmpeg-python==0.2.0
 jaraco.docker==2.0
-packaging==21.3
+packaging==22.0
 pathos==0.2.8
 peewee==3.14.7
 ping3==3.0.2
 pyarr==5.2.0
 qbittorrent-api==2023.7.52
 requests==2.31.0
 tomlkit==0.7.2
 
 [all]
-black==22.1.0
+black==24.3.0
 bump2version==1.0.1
 isort==5.10.1
 pip-tools==7.3.0
 pre-commit==3.3.3
 pyinstaller==5.13.1
 pyupgrade==2.31.0
 twine==3.7.1
 ujson==5.4.0
 upgrade-pip==0.1.4
 
 [dev]
-black==22.1.0
+black==24.3.0
 bump2version==1.0.1
 isort==5.10.1
 pip-tools==7.3.0
 pre-commit==3.3.3
 pyinstaller==5.13.1
 pyupgrade==2.31.0
 twine==3.7.1
```

### Comparing `qBitrr2-4.4.2/setup.cfg` & `qbitrr2-4.5.0/setup.cfg`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = qBitrr2
-version = 4.4.2
+version = 4.5.0
 description = "A simple Python script to talk to qBittorrent and Arr's"
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/Feramance/qBitrr
 author = Feramance
 author_email = fera@fera.wtf
 license = MIT
@@ -38,15 +38,15 @@
 install_requires = 
 	cachetools==5.3.2
 	colorama==0.4.4
 	coloredlogs==15.0.1
 	environ-config==23.2.0
 	ffmpeg-python==0.2.0
 	jaraco.docker==2.0
-	packaging==21.3
+	packaging==22.0
 	pathos==0.2.8
 	peewee==3.14.7
 	ping3==3.0.2
 	pyarr==5.2.0
 	qbittorrent-api==2023.7.52
 	requests==2.31.0
 	tomlkit==0.7.2
@@ -60,15 +60,15 @@
 
 [options.entry_points]
 console_scripts = 
 	qbitrr=qBitrr.main:run
 
 [options.extras_require]
 dev = 
-	black==22.1.0
+	black==24.3.0
 	bump2version==1.0.1
 	isort==5.10.1
 	pip-tools==7.3.0
 	pre-commit==3.3.3
 	pyinstaller==5.13.1
 	pyupgrade==2.31.0
 	twine==3.7.1
```

