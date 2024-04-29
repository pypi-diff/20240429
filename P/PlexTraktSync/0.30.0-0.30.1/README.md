# Comparing `tmp/plextraktsync-0.30.0.tar.gz` & `tmp/plextraktsync-0.30.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plextraktsync-0.30.0.tar", last modified: Sat Apr 27 18:24:03 2024, max compression
+gzip compressed data, was "plextraktsync-0.30.1.tar", last modified: Mon Apr 29 19:52:38 2024, max compression
```

## Comparing `plextraktsync-0.30.0.tar` & `plextraktsync-0.30.1.tar`

### file list

```diff
@@ -1,169 +1,170 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 18:24:03.533368 plextraktsync-0.30.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    30033 2024-04-27 18:24:03.533368 plextraktsync-0.30.0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 18:24:03.533368 plextraktsync-0.30.0/PlexTraktSync.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    30033 2024-04-27 18:24:03.000000 plextraktsync-0.30.0/PlexTraktSync.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5032 2024-04-27 18:24:03.000000 plextraktsync-0.30.0/PlexTraktSync.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-27 18:24:03.000000 plextraktsync-0.30.0/PlexTraktSync.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-27 18:24:03.000000 plextraktsync-0.30.0/PlexTraktSync.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1297 2024-04-27 18:24:03.000000 plextraktsync-0.30.0/PlexTraktSync.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-27 18:24:03.000000 plextraktsync-0.30.0/PlexTraktSync.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)    26812 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 18:24:03.513368 plextraktsync-0.30.0/plextraktsync/
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/plextraktsync/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      334 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/plextraktsync/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8307 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/plextraktsync/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 18:24:03.517368 plextraktsync-0.30.0/plextraktsync/commands/
--rw-r--r--   0 runner    (1001) docker     (127)      683 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/plextraktsync/commands/bug_report.py
--rw-r--r--   0 runner    (1001) docker     (127)     3314 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/plextraktsync/commands/cache.py
--rw-r--r--   0 runner    (1001) docker     (127)      759 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/plextraktsync/commands/clear_collections.py
--rw-r--r--   0 runner    (1001) docker     (127)      806 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/plextraktsync/commands/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2862 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/plextraktsync/commands/download.py
--rw-r--r--   0 runner    (1001) docker     (127)     2302 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/plextraktsync/commands/imdb_import.py
--rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/plextraktsync/commands/info.py
--rw-r--r--   0 runner    (1001) docker     (127)     3591 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/plextraktsync/commands/inspect.py
--rw-r--r--   0 runner    (1001) docker     (127)      826 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/plextraktsync/commands/login.py
--rw-r--r--   0 runner    (1001) docker     (127)     7212 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/plextraktsync/commands/plex_login.py
--rw-r--r--   0 runner    (1001) docker     (127)     1361 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/plextraktsync/commands/self_update.py
--rw-r--r--   0 runner    (1001) docker     (127)     2106 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/plextraktsync/commands/sync.py
--rw-r--r--   0 runner    (1001) docker     (127)     2228 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/plextraktsync/commands/trakt_login.py
--rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/plextraktsync/commands/unmatched.py
--rw-r--r--   0 runner    (1001) docker     (127)      914 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/plextraktsync/commands/watch.py
--rw-r--r--   0 runner    (1001) docker     (127)      690 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/plextraktsync/commands/watched_shows.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 18:24:03.517368 plextraktsync-0.30.0/plextraktsync/config/
--rw-r--r--   0 runner    (1001) docker     (127)     5729 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/plextraktsync/config/Config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/plextraktsync/config/ConfigLoader.py
--rw-r--r--   0 runner    (1001) docker     (127)      422 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/plextraktsync/config/ConfigMergeMixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     6402 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/plextraktsync/config/HttpCacheConfig.py
--rw-r--r--   0 runner    (1001) docker     (127)      848 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/plextraktsync/config/PlexServerConfig.py
--rw-r--r--   0 runner    (1001) docker     (127)      433 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/plextraktsync/config/RunConfig.py
--rw-r--r--   0 runner    (1001) docker     (127)     2069 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/plextraktsync/config/ServerConfigFactory.py
--rw-r--r--   0 runner    (1001) docker     (127)     3050 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/plextraktsync/config/SyncConfig.py
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/plextraktsync/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4022 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/plextraktsync/config.default.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 18:24:03.517368 plextraktsync-0.30.0/plextraktsync/decorators/
--rw-r--r--   0 runner    (1001) docker     (127)      452 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/plextraktsync/decorators/flatten.py
--rw-r--r--   0 runner    (1001) docker     (127)      569 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/plextraktsync/decorators/measure_time.py
--rw-r--r--   0 runner    (1001) docker     (127)      265 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/plextraktsync/decorators/memoize.py
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/plextraktsync/decorators/nocache.py
--rw-r--r--   0 runner    (1001) docker     (127)     1434 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/plextraktsync/decorators/rate_limit.py
--rw-r--r--   0 runner    (1001) docker     (127)     2093 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/plextraktsync/decorators/retry.py
--rw-r--r--   0 runner    (1001) docker     (127)      462 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/plextraktsync/decorators/time_limit.py
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/plextraktsync/factory.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 18:24:03.517368 plextraktsync-0.30.0/plextraktsync/logger/
--rw-r--r--   0 runner    (1001) docker     (127)     1966 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/plextraktsync/logger/filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1532 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/plextraktsync/logger/init.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 18:24:03.517368 plextraktsync-0.30.0/plextraktsync/media/
--rw-r--r--   0 runner    (1001) docker     (127)     7148 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/plextraktsync/media/Media.py
--rw-r--r--   0 runner    (1001) docker     (127)     3454 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/plextraktsync/media/MediaFactory.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 18:24:03.521368 plextraktsync-0.30.0/plextraktsync/mixin/
--rw-r--r--   0 runner    (1001) docker     (127)      552 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/plextraktsync/mixin/ChangeNotifier.py
--rw-r--r--   0 runner    (1001) docker     (127)      259 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/plextraktsync/mixin/RichMarkup.py
--rw-r--r--   0 runner    (1001) docker     (127)      388 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/plextraktsync/mixin/SetWindowTitle.py
--rw-r--r--   0 runner    (1001) docker     (127)      309 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/plextraktsync/path.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 18:24:03.521368 plextraktsync-0.30.0/plextraktsync/plan/
--rw-r--r--   0 runner    (1001) docker     (127)     1774 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/plextraktsync/plan/WalkConfig.py
--rw-r--r--   0 runner    (1001) docker     (127)      418 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/plextraktsync/plan/WalkPlan.py
--rw-r--r--   0 runner    (1001) docker     (127)     4275 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/plextraktsync/plan/WalkPlanner.py
--rw-r--r--   0 runner    (1001) docker     (127)     7152 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/plextraktsync/plan/Walker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 18:24:03.525368 plextraktsync-0.30.0/plextraktsync/plex/
--rw-r--r--   0 runner    (1001) docker     (127)     8811 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/plextraktsync/plex/PlexApi.py
--rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/plextraktsync/plex/PlexAudioCodec.py
--rw-r--r--   0 runner    (1001) docker     (127)     3345 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/plextraktsync/plex/PlexGuid.py
--rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/plextraktsync/plex/PlexGuidProvider.py
--rw-r--r--   0 runner    (1001) docker     (127)      439 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/plextraktsync/plex/PlexGuidProviderIMDB.py
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/plextraktsync/plex/PlexGuidProviderLocal.py
--rw-r--r--   0 runner    (1001) docker     (127)      592 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/plextraktsync/plex/PlexGuidProviderMbid.py
--rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/plextraktsync/plex/PlexGuidProviderTMDB.py
--rw-r--r--   0 runner    (1001) docker     (127)      463 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/plextraktsync/plex/PlexGuidProviderTVDB.py
--rw-r--r--   0 runner    (1001) docker     (127)      897 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/plextraktsync/plex/PlexId.py
--rw-r--r--   0 runner    (1001) docker     (127)     2541 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/plextraktsync/plex/PlexIdFactory.py
--rw-r--r--   0 runner    (1001) docker     (127)    11251 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/plextraktsync/plex/PlexLibraryItem.py
--rw-r--r--   0 runner    (1001) docker     (127)     1725 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/plextraktsync/plex/PlexLibrarySection.py
--rw-r--r--   0 runner    (1001) docker     (127)     3720 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/plextraktsync/plex/PlexPlaylist.py
--rw-r--r--   0 runner    (1001) docker     (127)      491 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/plextraktsync/plex/PlexPlaylistCollection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1841 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/plextraktsync/plex/PlexRatings.py
--rw-r--r--   0 runner    (1001) docker     (127)     1449 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/plextraktsync/plex/PlexSectionPager.py
--rw-r--r--   0 runner    (1001) docker     (127)     3132 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/plextraktsync/plex/PlexServerConnection.py
--rw-r--r--   0 runner    (1001) docker     (127)      898 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/plextraktsync/plex/PlexWatchList.py
--rw-r--r--   0 runner    (1001) docker     (127)      645 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/plextraktsync/plex/SessionCollection.py
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/plextraktsync/plex/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 18:24:03.525368 plextraktsync-0.30.0/plextraktsync/plugin/
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/plextraktsync/plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/plextraktsync/plugin/plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     4483 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/plextraktsync/pytrakt_extensions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 18:24:03.525368 plextraktsync-0.30.0/plextraktsync/queue/
--rw-r--r--   0 runner    (1001) docker     (127)     1845 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/plextraktsync/queue/BackgroundTask.py
--rw-r--r--   0 runner    (1001) docker     (127)     1673 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/plextraktsync/queue/Queue.py
--rw-r--r--   0 runner    (1001) docker     (127)     1827 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/plextraktsync/queue/TraktBatchWorker.py
--rw-r--r--   0 runner    (1001) docker     (127)     1410 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/plextraktsync/queue/TraktMarkWatchedWorker.py
--rw-r--r--   0 runner    (1001) docker     (127)     1779 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/plextraktsync/queue/TraktScrobbleWorker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 18:24:03.525368 plextraktsync-0.30.0/plextraktsync/rich/
--rw-r--r--   0 runner    (1001) docker     (127)      959 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/plextraktsync/rich/RichHighlighter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1851 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/plextraktsync/rich/RichProgressBar.py
--rw-r--r--   0 runner    (1001) docker     (127)      356 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/plextraktsync/style.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 18:24:03.525368 plextraktsync-0.30.0/plextraktsync/sync/
--rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/plextraktsync/sync/AddCollectionPlugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     2100 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/plextraktsync/sync/ClearCollectedPlugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/plextraktsync/sync/LikedListsPlugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1905 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/plextraktsync/sync/Sync.py
--rw-r--r--   0 runner    (1001) docker     (127)     2990 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/plextraktsync/sync/SyncRatingsPlugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     2037 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/plextraktsync/sync/SyncWatchedPlugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     5276 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/plextraktsync/sync/WatchListPlugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1715 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/plextraktsync/sync/WatchProgressPlugin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 18:24:03.525368 plextraktsync-0.30.0/plextraktsync/sync/plugin/
--rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/plextraktsync/sync/plugin/SyncPluginInterface.py
--rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/plextraktsync/sync/plugin/SyncPluginManager.py
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/plextraktsync/sync/plugin/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 18:24:03.529368 plextraktsync-0.30.0/plextraktsync/trakt/
--rw-r--r--   0 runner    (1001) docker     (127)      485 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/plextraktsync/trakt/PartialTraktMedia.py
--rw-r--r--   0 runner    (1001) docker     (127)      671 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/plextraktsync/trakt/ScrobblerCollection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1281 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/plextraktsync/trakt/ScrobblerProxy.py
--rw-r--r--   0 runner    (1001) docker     (127)    10522 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/plextraktsync/trakt/TraktApi.py
--rw-r--r--   0 runner    (1001) docker     (127)      483 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/plextraktsync/trakt/TraktItem.py
--rw-r--r--   0 runner    (1001) docker     (127)     3276 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/plextraktsync/trakt/TraktLookup.py
--rw-r--r--   0 runner    (1001) docker     (127)      858 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/plextraktsync/trakt/TraktRatingCollection.py
--rw-r--r--   0 runner    (1001) docker     (127)     3584 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/plextraktsync/trakt/TraktUserList.py
--rw-r--r--   0 runner    (1001) docker     (127)     1577 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/plextraktsync/trakt/TraktUserListCollection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/plextraktsync/trakt/TraktWatchlist.py
--rw-r--r--   0 runner    (1001) docker     (127)      528 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/plextraktsync/trakt/WatchProgress.py
--rw-r--r--   0 runner    (1001) docker     (127)      349 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/plextraktsync/trakt/trakt_set.py
--rw-r--r--   0 runner    (1001) docker     (127)      282 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/plextraktsync/trakt/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 18:24:03.529368 plextraktsync-0.30.0/plextraktsync/util/
--rw-r--r--   0 runner    (1001) docker     (127)     9024 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/plextraktsync/util/Factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     1707 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/plextraktsync/util/Path.py
--rw-r--r--   0 runner    (1001) docker     (127)     1380 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/plextraktsync/util/Rating.py
--rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/plextraktsync/util/Timer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1972 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/plextraktsync/util/Version.py
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/plextraktsync/util/execp.py
--rw-r--r--   0 runner    (1001) docker     (127)      305 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/plextraktsync/util/execx.py
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/plextraktsync/util/expand_id.py
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/plextraktsync/util/git_version_info.py
--rw-r--r--   0 runner    (1001) docker     (127)      615 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/plextraktsync/util/local_url.py
--rw-r--r--   0 runner    (1001) docker     (127)      513 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/plextraktsync/util/openurl.py
--rw-r--r--   0 runner    (1001) docker     (127)     1836 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/plextraktsync/util/packaging.py
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/plextraktsync/util/parse_date.py
--rw-r--r--   0 runner    (1001) docker     (127)      786 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/plextraktsync/util/remove_empty_values.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 18:24:03.533368 plextraktsync-0.30.0/plextraktsync/watch/
--rw-r--r--   0 runner    (1001) docker     (127)     1951 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/plextraktsync/watch/EventDispatcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     1316 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/plextraktsync/watch/EventFactory.py
--rw-r--r--   0 runner    (1001) docker     (127)     2069 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/plextraktsync/watch/ProgressBar.py
--rw-r--r--   0 runner    (1001) docker     (127)     6851 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/plextraktsync/watch/WatchStateUpdater.py
--rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/plextraktsync/watch/WebSocketListener.py
--rw-r--r--   0 runner    (1001) docker     (127)     1906 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/plextraktsync/watch/events.py
--rw-r--r--   0 runner    (1001) docker     (127)      155 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1830 2024-04-27 18:24:01.000000 plextraktsync-0.30.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1559 2024-04-27 18:24:03.533368 plextraktsync-0.30.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 18:24:03.533368 plextraktsync-0.30.0/tests/
--rwxr-xr-x   0 runner    (1001) docker     (127)     1923 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/tests/test_collection_metadata.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1443 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/tests/test_config.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2703 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/tests/test_events.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      341 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/tests/test_logger.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      977 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/tests/test_new_agent.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2104 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/tests/test_plex_id.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      529 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/tests/test_rating.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      503 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/tests/test_threading.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1174 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/tests/test_timer.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      572 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/tests/test_trakt_progress.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3584 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/tests/test_tv_lookup.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1977 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/tests/test_walker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:52:38.486534 plextraktsync-0.30.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    30005 2024-04-29 19:52:38.486534 plextraktsync-0.30.1/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:52:38.486534 plextraktsync-0.30.1/PlexTraktSync.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    30005 2024-04-29 19:52:38.000000 plextraktsync-0.30.1/PlexTraktSync.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5071 2024-04-29 19:52:38.000000 plextraktsync-0.30.1/PlexTraktSync.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 19:52:38.000000 plextraktsync-0.30.1/PlexTraktSync.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-29 19:52:38.000000 plextraktsync-0.30.1/PlexTraktSync.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1297 2024-04-29 19:52:38.000000 plextraktsync-0.30.1/PlexTraktSync.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-29 19:52:38.000000 plextraktsync-0.30.1/PlexTraktSync.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    26812 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:52:38.466534 plextraktsync-0.30.1/plextraktsync/
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-29 19:52:35.000000 plextraktsync-0.30.1/plextraktsync/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/plextraktsync/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8307 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/plextraktsync/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:52:38.466534 plextraktsync-0.30.1/plextraktsync/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)      683 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/plextraktsync/commands/bug_report.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3314 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/plextraktsync/commands/cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)      759 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/plextraktsync/commands/clear_collections.py
+-rw-r--r--   0 runner    (1001) docker     (127)      806 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/plextraktsync/commands/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2862 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/plextraktsync/commands/download.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2302 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/plextraktsync/commands/imdb_import.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/plextraktsync/commands/info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3591 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/plextraktsync/commands/inspect.py
+-rw-r--r--   0 runner    (1001) docker     (127)      826 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/plextraktsync/commands/login.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7212 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/plextraktsync/commands/plex_login.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1361 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/plextraktsync/commands/self_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2106 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/plextraktsync/commands/sync.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2228 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/plextraktsync/commands/trakt_login.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/plextraktsync/commands/unmatched.py
+-rw-r--r--   0 runner    (1001) docker     (127)      914 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/plextraktsync/commands/watch.py
+-rw-r--r--   0 runner    (1001) docker     (127)      690 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/plextraktsync/commands/watched_shows.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:52:38.470534 plextraktsync-0.30.1/plextraktsync/config/
+-rw-r--r--   0 runner    (1001) docker     (127)     5729 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/plextraktsync/config/Config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/plextraktsync/config/ConfigLoader.py
+-rw-r--r--   0 runner    (1001) docker     (127)      422 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/plextraktsync/config/ConfigMergeMixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6402 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/plextraktsync/config/HttpCacheConfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)      848 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/plextraktsync/config/PlexServerConfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)      433 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/plextraktsync/config/RunConfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2069 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/plextraktsync/config/ServerConfigFactory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3050 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/plextraktsync/config/SyncConfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/plextraktsync/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4022 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/plextraktsync/config.default.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:52:38.470534 plextraktsync-0.30.1/plextraktsync/decorators/
+-rw-r--r--   0 runner    (1001) docker     (127)      452 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/plextraktsync/decorators/flatten.py
+-rw-r--r--   0 runner    (1001) docker     (127)      767 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/plextraktsync/decorators/measure_time.py
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/plextraktsync/decorators/memoize.py
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/plextraktsync/decorators/nocache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1434 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/plextraktsync/decorators/rate_limit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2093 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/plextraktsync/decorators/retry.py
+-rw-r--r--   0 runner    (1001) docker     (127)      462 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/plextraktsync/decorators/time_limit.py
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/plextraktsync/factory.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:52:38.470534 plextraktsync-0.30.1/plextraktsync/logger/
+-rw-r--r--   0 runner    (1001) docker     (127)     1966 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/plextraktsync/logger/filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1532 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/plextraktsync/logger/init.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:52:38.470534 plextraktsync-0.30.1/plextraktsync/media/
+-rw-r--r--   0 runner    (1001) docker     (127)     7148 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/plextraktsync/media/Media.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3454 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/plextraktsync/media/MediaFactory.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:52:38.470534 plextraktsync-0.30.1/plextraktsync/mixin/
+-rw-r--r--   0 runner    (1001) docker     (127)      552 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/plextraktsync/mixin/ChangeNotifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/plextraktsync/mixin/RichMarkup.py
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/plextraktsync/mixin/SetWindowTitle.py
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/plextraktsync/path.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:52:38.470534 plextraktsync-0.30.1/plextraktsync/plan/
+-rw-r--r--   0 runner    (1001) docker     (127)     1774 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/plextraktsync/plan/WalkConfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)      418 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/plextraktsync/plan/WalkPlan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4275 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/plextraktsync/plan/WalkPlanner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7152 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/plextraktsync/plan/Walker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:52:38.474534 plextraktsync-0.30.1/plextraktsync/plex/
+-rw-r--r--   0 runner    (1001) docker     (127)     8811 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/plextraktsync/plex/PlexApi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/plextraktsync/plex/PlexAudioCodec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3345 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/plextraktsync/plex/PlexGuid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/plextraktsync/plex/PlexGuidProvider.py
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/plextraktsync/plex/PlexGuidProviderIMDB.py
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/plextraktsync/plex/PlexGuidProviderLocal.py
+-rw-r--r--   0 runner    (1001) docker     (127)      592 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/plextraktsync/plex/PlexGuidProviderMbid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/plextraktsync/plex/PlexGuidProviderTMDB.py
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/plextraktsync/plex/PlexGuidProviderTVDB.py
+-rw-r--r--   0 runner    (1001) docker     (127)      897 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/plextraktsync/plex/PlexId.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2541 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/plextraktsync/plex/PlexIdFactory.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11251 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/plextraktsync/plex/PlexLibraryItem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1725 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/plextraktsync/plex/PlexLibrarySection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3720 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/plextraktsync/plex/PlexPlaylist.py
+-rw-r--r--   0 runner    (1001) docker     (127)      491 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/plextraktsync/plex/PlexPlaylistCollection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1841 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/plextraktsync/plex/PlexRatings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1449 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/plextraktsync/plex/PlexSectionPager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3132 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/plextraktsync/plex/PlexServerConnection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      898 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/plextraktsync/plex/PlexWatchList.py
+-rw-r--r--   0 runner    (1001) docker     (127)      645 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/plextraktsync/plex/SessionCollection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/plextraktsync/plex/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:52:38.474534 plextraktsync-0.30.1/plextraktsync/plugin/
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/plextraktsync/plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/plextraktsync/plugin/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4483 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/plextraktsync/pytrakt_extensions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:52:38.474534 plextraktsync-0.30.1/plextraktsync/queue/
+-rw-r--r--   0 runner    (1001) docker     (127)     1845 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/plextraktsync/queue/BackgroundTask.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1673 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/plextraktsync/queue/Queue.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1827 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/plextraktsync/queue/TraktBatchWorker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1410 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/plextraktsync/queue/TraktMarkWatchedWorker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1779 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/plextraktsync/queue/TraktScrobbleWorker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:52:38.474534 plextraktsync-0.30.1/plextraktsync/rich/
+-rw-r--r--   0 runner    (1001) docker     (127)      959 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/plextraktsync/rich/RichHighlighter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1851 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/plextraktsync/rich/RichProgressBar.py
+-rw-r--r--   0 runner    (1001) docker     (127)      356 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/plextraktsync/style.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:52:38.478534 plextraktsync-0.30.1/plextraktsync/sync/
+-rw-r--r--   0 runner    (1001) docker     (127)      989 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/plextraktsync/sync/AddCollectionPlugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2088 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/plextraktsync/sync/ClearCollectedPlugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      979 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/plextraktsync/sync/LikedListsPlugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/plextraktsync/sync/Sync.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2865 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/plextraktsync/sync/SyncRatingsPlugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1953 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/plextraktsync/sync/SyncWatchedPlugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/plextraktsync/sync/TraktListsPlugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5037 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/plextraktsync/sync/WatchListPlugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1673 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/plextraktsync/sync/WatchProgressPlugin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:52:38.478534 plextraktsync-0.30.1/plextraktsync/sync/plugin/
+-rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/plextraktsync/sync/plugin/SyncPluginInterface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2036 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/plextraktsync/sync/plugin/SyncPluginManager.py
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/plextraktsync/sync/plugin/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:52:38.478534 plextraktsync-0.30.1/plextraktsync/trakt/
+-rw-r--r--   0 runner    (1001) docker     (127)      485 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/plextraktsync/trakt/PartialTraktMedia.py
+-rw-r--r--   0 runner    (1001) docker     (127)      671 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/plextraktsync/trakt/ScrobblerCollection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1281 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/plextraktsync/trakt/ScrobblerProxy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10522 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/plextraktsync/trakt/TraktApi.py
+-rw-r--r--   0 runner    (1001) docker     (127)      483 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/plextraktsync/trakt/TraktItem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3276 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/plextraktsync/trakt/TraktLookup.py
+-rw-r--r--   0 runner    (1001) docker     (127)      858 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/plextraktsync/trakt/TraktRatingCollection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3584 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/plextraktsync/trakt/TraktUserList.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1577 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/plextraktsync/trakt/TraktUserListCollection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/plextraktsync/trakt/TraktWatchlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)      528 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/plextraktsync/trakt/WatchProgress.py
+-rw-r--r--   0 runner    (1001) docker     (127)      349 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/plextraktsync/trakt/trakt_set.py
+-rw-r--r--   0 runner    (1001) docker     (127)      282 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/plextraktsync/trakt/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:52:38.482534 plextraktsync-0.30.1/plextraktsync/util/
+-rw-r--r--   0 runner    (1001) docker     (127)     9024 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/plextraktsync/util/Factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1707 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/plextraktsync/util/Path.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1380 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/plextraktsync/util/Rating.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/plextraktsync/util/Timer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1972 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/plextraktsync/util/Version.py
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/plextraktsync/util/execp.py
+-rw-r--r--   0 runner    (1001) docker     (127)      305 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/plextraktsync/util/execx.py
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/plextraktsync/util/expand_id.py
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/plextraktsync/util/git_version_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)      615 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/plextraktsync/util/local_url.py
+-rw-r--r--   0 runner    (1001) docker     (127)      513 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/plextraktsync/util/openurl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1836 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/plextraktsync/util/packaging.py
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/plextraktsync/util/parse_date.py
+-rw-r--r--   0 runner    (1001) docker     (127)      786 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/plextraktsync/util/remove_empty_values.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:52:38.482534 plextraktsync-0.30.1/plextraktsync/watch/
+-rw-r--r--   0 runner    (1001) docker     (127)     1951 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/plextraktsync/watch/EventDispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1316 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/plextraktsync/watch/EventFactory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2069 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/plextraktsync/watch/ProgressBar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6851 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/plextraktsync/watch/WatchStateUpdater.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/plextraktsync/watch/WebSocketListener.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1906 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/plextraktsync/watch/events.py
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1802 2024-04-29 19:52:36.000000 plextraktsync-0.30.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1559 2024-04-29 19:52:38.486534 plextraktsync-0.30.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:52:38.486534 plextraktsync-0.30.1/tests/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1923 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/tests/test_collection_metadata.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1443 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/tests/test_config.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2703 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/tests/test_events.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      341 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/tests/test_logger.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      977 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/tests/test_new_agent.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2104 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/tests/test_plex_id.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      529 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/tests/test_rating.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      503 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/tests/test_threading.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1174 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/tests/test_timer.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      572 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/tests/test_trakt_progress.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3584 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/tests/test_tv_lookup.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1977 2024-04-29 19:52:34.000000 plextraktsync-0.30.1/tests/test_walker.py
```

### Comparing `plextraktsync-0.30.0/LICENSE` & `plextraktsync-0.30.1/LICENSE`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.0/PKG-INFO` & `plextraktsync-0.30.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PlexTraktSync
-Version: 0.30.0
+Version: 0.30.1
 Summary: Plex-Trakt-Sync is a two-way-sync between trakt.tv and Plex Media Server
 Home-page: https://github.com/Taxel/PlexTraktSync
 License: MIT
 Project-URL: Bug Tracker, https://github.com/Taxel/PlexTraktSync/issues
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -20,25 +20,25 @@
 License-File: LICENSE
 Requires-Dist: attrs==23.2.0; python_version >= "3.7"
 Requires-Dist: cattrs==23.2.3; python_version >= "3.7" and python_version >= "3.8"
 Requires-Dist: certifi==2024.2.2; python_version >= "3.6"
 Requires-Dist: charset-normalizer==3.3.2; python_full_version >= "3.7.0"
 Requires-Dist: click==8.1.7; python_version >= "3.7"
 Requires-Dist: deprecated==1.2.14; python_version >= "2.7" and python_version not in "3.0, 3.1, 3.2, 3.3"
-Requires-Dist: exceptiongroup==1.2.0; python_version < "3.11"
+Requires-Dist: exceptiongroup==1.2.1; python_version >= "3.7"
 Requires-Dist: humanize==4.9.0; python_version >= "3.8"
 Requires-Dist: idna==3.7; python_version >= "3.5"
 Requires-Dist: inquirerpy==0.3.4; python_version >= "3.7" and python_version < "4.0"
 Requires-Dist: markdown-it-py==3.0.0; python_version >= "3.7" and python_version >= "3.8"
 Requires-Dist: mdurl==0.1.2; python_version >= "3.7"
 Requires-Dist: oauthlib==3.2.2; python_version >= "3.6"
 Requires-Dist: pfzy==0.3.4; python_version >= "3.7" and python_version < "4.0"
-Requires-Dist: platformdirs==4.2.0; python_version >= "3.7" and python_version >= "3.8"
-Requires-Dist: plexapi==4.15.11; python_version >= "3.8"
-Requires-Dist: pluggy==1.4.0; python_version >= "3.8"
+Requires-Dist: platformdirs==4.2.1; python_version >= "3.8"
+Requires-Dist: plexapi==4.15.12; python_version >= "3.8"
+Requires-Dist: pluggy==1.5.0; python_version >= "3.8"
 Requires-Dist: prompt-toolkit==3.0.43; python_full_version >= "3.7.0"
 Requires-Dist: pygments==2.17.2; python_version >= "3.7"
 Requires-Dist: python-dotenv==1.0.1; python_version >= "3.8"
 Requires-Dist: python-git-info==0.8.3
 Requires-Dist: pytimeparse==1.1.8
 Requires-Dist: pytrakt==3.4.32
 Requires-Dist: pyyaml==6.0.1; python_version >= "3.6"
@@ -48,15 +48,15 @@
 Requires-Dist: rich==13.7.1; python_full_version >= "3.7.0"
 Requires-Dist: six==1.16.0; python_version >= "2.7" and python_version not in "3.0, 3.1, 3.2, 3.3" and python_version >= "3.4"
 Requires-Dist: tqdm==4.66.2; python_version >= "3.7"
 Requires-Dist: typing-extensions==4.11.0; python_version < "3.11"
 Requires-Dist: url-normalize==1.4.3; python_version >= "2.7" and python_version not in "3.0, 3.1, 3.2, 3.3, 3.4, 3.5" and python_version >= "3.6"
 Requires-Dist: urllib3==2.2.1; python_version >= "3.8"
 Requires-Dist: wcwidth==0.2.13
-Requires-Dist: websocket-client==1.7.0; python_version >= "3.8"
+Requires-Dist: websocket-client==1.8.0; python_version >= "3.8"
 Requires-Dist: wrapt==1.16.0; python_version >= "3.5" and python_version >= "3.6"
 
 # Plex-Trakt-Sync
 
 ![Python Versions][python-versions-badge]
 
 This project adds a two-way-sync between trakt.tv and Plex Media Server. It
```

### Comparing `plextraktsync-0.30.0/PlexTraktSync.egg-info/PKG-INFO` & `plextraktsync-0.30.1/PlexTraktSync.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PlexTraktSync
-Version: 0.30.0
+Version: 0.30.1
 Summary: Plex-Trakt-Sync is a two-way-sync between trakt.tv and Plex Media Server
 Home-page: https://github.com/Taxel/PlexTraktSync
 License: MIT
 Project-URL: Bug Tracker, https://github.com/Taxel/PlexTraktSync/issues
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -20,25 +20,25 @@
 License-File: LICENSE
 Requires-Dist: attrs==23.2.0; python_version >= "3.7"
 Requires-Dist: cattrs==23.2.3; python_version >= "3.7" and python_version >= "3.8"
 Requires-Dist: certifi==2024.2.2; python_version >= "3.6"
 Requires-Dist: charset-normalizer==3.3.2; python_full_version >= "3.7.0"
 Requires-Dist: click==8.1.7; python_version >= "3.7"
 Requires-Dist: deprecated==1.2.14; python_version >= "2.7" and python_version not in "3.0, 3.1, 3.2, 3.3"
-Requires-Dist: exceptiongroup==1.2.0; python_version < "3.11"
+Requires-Dist: exceptiongroup==1.2.1; python_version >= "3.7"
 Requires-Dist: humanize==4.9.0; python_version >= "3.8"
 Requires-Dist: idna==3.7; python_version >= "3.5"
 Requires-Dist: inquirerpy==0.3.4; python_version >= "3.7" and python_version < "4.0"
 Requires-Dist: markdown-it-py==3.0.0; python_version >= "3.7" and python_version >= "3.8"
 Requires-Dist: mdurl==0.1.2; python_version >= "3.7"
 Requires-Dist: oauthlib==3.2.2; python_version >= "3.6"
 Requires-Dist: pfzy==0.3.4; python_version >= "3.7" and python_version < "4.0"
-Requires-Dist: platformdirs==4.2.0; python_version >= "3.7" and python_version >= "3.8"
-Requires-Dist: plexapi==4.15.11; python_version >= "3.8"
-Requires-Dist: pluggy==1.4.0; python_version >= "3.8"
+Requires-Dist: platformdirs==4.2.1; python_version >= "3.8"
+Requires-Dist: plexapi==4.15.12; python_version >= "3.8"
+Requires-Dist: pluggy==1.5.0; python_version >= "3.8"
 Requires-Dist: prompt-toolkit==3.0.43; python_full_version >= "3.7.0"
 Requires-Dist: pygments==2.17.2; python_version >= "3.7"
 Requires-Dist: python-dotenv==1.0.1; python_version >= "3.8"
 Requires-Dist: python-git-info==0.8.3
 Requires-Dist: pytimeparse==1.1.8
 Requires-Dist: pytrakt==3.4.32
 Requires-Dist: pyyaml==6.0.1; python_version >= "3.6"
@@ -48,15 +48,15 @@
 Requires-Dist: rich==13.7.1; python_full_version >= "3.7.0"
 Requires-Dist: six==1.16.0; python_version >= "2.7" and python_version not in "3.0, 3.1, 3.2, 3.3" and python_version >= "3.4"
 Requires-Dist: tqdm==4.66.2; python_version >= "3.7"
 Requires-Dist: typing-extensions==4.11.0; python_version < "3.11"
 Requires-Dist: url-normalize==1.4.3; python_version >= "2.7" and python_version not in "3.0, 3.1, 3.2, 3.3, 3.4, 3.5" and python_version >= "3.6"
 Requires-Dist: urllib3==2.2.1; python_version >= "3.8"
 Requires-Dist: wcwidth==0.2.13
-Requires-Dist: websocket-client==1.7.0; python_version >= "3.8"
+Requires-Dist: websocket-client==1.8.0; python_version >= "3.8"
 Requires-Dist: wrapt==1.16.0; python_version >= "3.5" and python_version >= "3.6"
 
 # Plex-Trakt-Sync
 
 ![Python Versions][python-versions-badge]
 
 This project adds a two-way-sync between trakt.tv and Plex Media Server. It
```

### Comparing `plextraktsync-0.30.0/PlexTraktSync.egg-info/SOURCES.txt` & `plextraktsync-0.30.1/PlexTraktSync.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -92,14 +92,15 @@
 plextraktsync/rich/RichProgressBar.py
 plextraktsync/sync/AddCollectionPlugin.py
 plextraktsync/sync/ClearCollectedPlugin.py
 plextraktsync/sync/LikedListsPlugin.py
 plextraktsync/sync/Sync.py
 plextraktsync/sync/SyncRatingsPlugin.py
 plextraktsync/sync/SyncWatchedPlugin.py
+plextraktsync/sync/TraktListsPlugin.py
 plextraktsync/sync/WatchListPlugin.py
 plextraktsync/sync/WatchProgressPlugin.py
 plextraktsync/sync/plugin/SyncPluginInterface.py
 plextraktsync/sync/plugin/SyncPluginManager.py
 plextraktsync/sync/plugin/__init__.py
 plextraktsync/trakt/PartialTraktMedia.py
 plextraktsync/trakt/ScrobblerCollection.py
```

### Comparing `plextraktsync-0.30.0/PlexTraktSync.egg-info/requires.txt` & `plextraktsync-0.30.1/PlexTraktSync.egg-info/requires.txt`

 * *Files 8% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 
 [:python_full_version >= "3.7.0"]
 charset-normalizer==3.3.2
 prompt-toolkit==3.0.43
 rich==13.7.1
 
 [:python_version < "3.11"]
-exceptiongroup==1.2.0
 typing-extensions==4.11.0
 
 [:python_version >= "2.7" and python_version not in "3.0, 3.1, 3.2, 3.3"]
 deprecated==1.2.14
 
 [:python_version >= "2.7" and python_version not in "3.0, 3.1, 3.2, 3.3" and python_version >= "3.4"]
 six==1.16.0
@@ -34,29 +33,30 @@
 certifi==2024.2.2
 oauthlib==3.2.2
 pyyaml==6.0.1
 
 [:python_version >= "3.7"]
 attrs==23.2.0
 click==8.1.7
+exceptiongroup==1.2.1
 mdurl==0.1.2
 pygments==2.17.2
 requests==2.31.0
 tqdm==4.66.2
 
 [:python_version >= "3.7" and python_version < "4.0"]
 inquirerpy==0.3.4
 pfzy==0.3.4
 
 [:python_version >= "3.7" and python_version >= "3.8"]
 cattrs==23.2.3
 markdown-it-py==3.0.0
-platformdirs==4.2.0
 
 [:python_version >= "3.8"]
 humanize==4.9.0
-plexapi==4.15.11
-pluggy==1.4.0
+platformdirs==4.2.1
+plexapi==4.15.12
+pluggy==1.5.0
 python-dotenv==1.0.1
 requests-cache==1.2.0
 urllib3==2.2.1
-websocket-client==1.7.0
+websocket-client==1.8.0
```

### Comparing `plextraktsync-0.30.0/README.md` & `plextraktsync-0.30.1/README.md`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.0/plextraktsync/cli.py` & `plextraktsync-0.30.1/plextraktsync/cli.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.0/plextraktsync/commands/bug_report.py` & `plextraktsync-0.30.1/plextraktsync/commands/bug_report.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.0/plextraktsync/commands/cache.py` & `plextraktsync-0.30.1/plextraktsync/commands/cache.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.0/plextraktsync/commands/clear_collections.py` & `plextraktsync-0.30.1/plextraktsync/commands/clear_collections.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.0/plextraktsync/commands/config.py` & `plextraktsync-0.30.1/plextraktsync/commands/config.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.0/plextraktsync/commands/download.py` & `plextraktsync-0.30.1/plextraktsync/commands/download.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.0/plextraktsync/commands/imdb_import.py` & `plextraktsync-0.30.1/plextraktsync/commands/imdb_import.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.0/plextraktsync/commands/info.py` & `plextraktsync-0.30.1/plextraktsync/commands/info.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.0/plextraktsync/commands/inspect.py` & `plextraktsync-0.30.1/plextraktsync/commands/inspect.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.0/plextraktsync/commands/login.py` & `plextraktsync-0.30.1/plextraktsync/commands/login.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.0/plextraktsync/commands/plex_login.py` & `plextraktsync-0.30.1/plextraktsync/commands/plex_login.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.0/plextraktsync/commands/self_update.py` & `plextraktsync-0.30.1/plextraktsync/commands/self_update.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.0/plextraktsync/commands/sync.py` & `plextraktsync-0.30.1/plextraktsync/commands/sync.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.0/plextraktsync/commands/trakt_login.py` & `plextraktsync-0.30.1/plextraktsync/commands/trakt_login.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.0/plextraktsync/commands/unmatched.py` & `plextraktsync-0.30.1/plextraktsync/commands/unmatched.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.0/plextraktsync/commands/watch.py` & `plextraktsync-0.30.1/plextraktsync/commands/watch.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.0/plextraktsync/commands/watched_shows.py` & `plextraktsync-0.30.1/plextraktsync/commands/watched_shows.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.0/plextraktsync/config/Config.py` & `plextraktsync-0.30.1/plextraktsync/config/Config.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.0/plextraktsync/config/ConfigLoader.py` & `plextraktsync-0.30.1/plextraktsync/config/ConfigLoader.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.0/plextraktsync/config/HttpCacheConfig.py` & `plextraktsync-0.30.1/plextraktsync/config/HttpCacheConfig.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.0/plextraktsync/config/PlexServerConfig.py` & `plextraktsync-0.30.1/plextraktsync/config/PlexServerConfig.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.0/plextraktsync/config/ServerConfigFactory.py` & `plextraktsync-0.30.1/plextraktsync/config/ServerConfigFactory.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.0/plextraktsync/config/SyncConfig.py` & `plextraktsync-0.30.1/plextraktsync/config/SyncConfig.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.0/plextraktsync/config.default.yml` & `plextraktsync-0.30.1/plextraktsync/config.default.yml`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.0/plextraktsync/decorators/measure_time.py` & `plextraktsync-0.30.1/plextraktsync/decorators/measure_time.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,23 +1,31 @@
+import inspect
 from contextlib import contextmanager
 from datetime import timedelta
 from time import monotonic
 
 from humanize.time import precisedelta
 
 from plextraktsync.factory import logging
 
-logger = logging.getLogger(__name__)
+default_logger = logging.getLogger(__name__)
 
 
 @contextmanager
-def measure_time(message, level=logging.INFO, **kwargs):
+def measure_time(message, *args, level=logging.INFO, logger=None, **kwargs):
     start = monotonic()
     yield
     delta = monotonic() - start
 
+    if inspect.ismethod(logger):
+        log = logger
+    else:
+        def log(*a, **kw):
+            (logger or default_logger).log(level, *a, **kw)
+
     minimum_unit = "microseconds" if delta < 1 else "seconds"
-    logger.log(
-        level,
-        f"{message} in " + precisedelta(timedelta(seconds=delta), minimum_unit=minimum_unit),
-        **kwargs
+    log(
+        f"{message} in %s",
+        precisedelta(timedelta(seconds=delta), minimum_unit=minimum_unit),
+        *args,
+        **kwargs,
     )
```

### Comparing `plextraktsync-0.30.0/plextraktsync/decorators/rate_limit.py` & `plextraktsync-0.30.1/plextraktsync/decorators/rate_limit.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.0/plextraktsync/decorators/retry.py` & `plextraktsync-0.30.1/plextraktsync/decorators/retry.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.0/plextraktsync/logger/filter.py` & `plextraktsync-0.30.1/plextraktsync/logger/filter.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.0/plextraktsync/logger/init.py` & `plextraktsync-0.30.1/plextraktsync/logger/init.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.0/plextraktsync/media/Media.py` & `plextraktsync-0.30.1/plextraktsync/media/Media.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.0/plextraktsync/media/MediaFactory.py` & `plextraktsync-0.30.1/plextraktsync/media/MediaFactory.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.0/plextraktsync/mixin/ChangeNotifier.py` & `plextraktsync-0.30.1/plextraktsync/mixin/ChangeNotifier.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.0/plextraktsync/plan/WalkConfig.py` & `plextraktsync-0.30.1/plextraktsync/plan/WalkConfig.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.0/plextraktsync/plan/WalkPlanner.py` & `plextraktsync-0.30.1/plextraktsync/plan/WalkPlanner.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.0/plextraktsync/plan/Walker.py` & `plextraktsync-0.30.1/plextraktsync/plan/Walker.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.0/plextraktsync/plex/PlexApi.py` & `plextraktsync-0.30.1/plextraktsync/plex/PlexApi.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.0/plextraktsync/plex/PlexAudioCodec.py` & `plextraktsync-0.30.1/plextraktsync/plex/PlexAudioCodec.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.0/plextraktsync/plex/PlexGuid.py` & `plextraktsync-0.30.1/plextraktsync/plex/PlexGuid.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.0/plextraktsync/plex/PlexGuidProvider.py` & `plextraktsync-0.30.1/plextraktsync/plex/PlexGuidProvider.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.0/plextraktsync/plex/PlexGuidProviderMbid.py` & `plextraktsync-0.30.1/plextraktsync/plex/PlexGuidProviderMbid.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.0/plextraktsync/plex/PlexGuidProviderTMDB.py` & `plextraktsync-0.30.1/plextraktsync/plex/PlexGuidProviderTMDB.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.0/plextraktsync/plex/PlexId.py` & `plextraktsync-0.30.1/plextraktsync/plex/PlexId.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.0/plextraktsync/plex/PlexIdFactory.py` & `plextraktsync-0.30.1/plextraktsync/plex/PlexIdFactory.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.0/plextraktsync/plex/PlexLibraryItem.py` & `plextraktsync-0.30.1/plextraktsync/plex/PlexLibraryItem.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.0/plextraktsync/plex/PlexLibrarySection.py` & `plextraktsync-0.30.1/plextraktsync/plex/PlexLibrarySection.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.0/plextraktsync/plex/PlexPlaylist.py` & `plextraktsync-0.30.1/plextraktsync/plex/PlexPlaylist.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.0/plextraktsync/plex/PlexRatings.py` & `plextraktsync-0.30.1/plextraktsync/plex/PlexRatings.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.0/plextraktsync/plex/PlexSectionPager.py` & `plextraktsync-0.30.1/plextraktsync/plex/PlexSectionPager.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.0/plextraktsync/plex/PlexServerConnection.py` & `plextraktsync-0.30.1/plextraktsync/plex/PlexServerConnection.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.0/plextraktsync/plex/PlexWatchList.py` & `plextraktsync-0.30.1/plextraktsync/plex/PlexWatchList.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.0/plextraktsync/plex/SessionCollection.py` & `plextraktsync-0.30.1/plextraktsync/plex/SessionCollection.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.0/plextraktsync/pytrakt_extensions.py` & `plextraktsync-0.30.1/plextraktsync/pytrakt_extensions.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.0/plextraktsync/queue/BackgroundTask.py` & `plextraktsync-0.30.1/plextraktsync/queue/BackgroundTask.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.0/plextraktsync/queue/Queue.py` & `plextraktsync-0.30.1/plextraktsync/queue/Queue.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.0/plextraktsync/queue/TraktBatchWorker.py` & `plextraktsync-0.30.1/plextraktsync/queue/TraktBatchWorker.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.0/plextraktsync/queue/TraktMarkWatchedWorker.py` & `plextraktsync-0.30.1/plextraktsync/queue/TraktMarkWatchedWorker.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.0/plextraktsync/queue/TraktScrobbleWorker.py` & `plextraktsync-0.30.1/plextraktsync/queue/TraktScrobbleWorker.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.0/plextraktsync/rich/RichHighlighter.py` & `plextraktsync-0.30.1/plextraktsync/rich/RichHighlighter.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.0/plextraktsync/rich/RichProgressBar.py` & `plextraktsync-0.30.1/plextraktsync/rich/RichProgressBar.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.0/plextraktsync/sync/AddCollectionPlugin.py` & `plextraktsync-0.30.1/plextraktsync/sync/AddCollectionPlugin.py`

 * *Files 19% similar despite different names*

```diff
@@ -2,28 +2,26 @@
 
 from typing import TYPE_CHECKING
 
 from plextraktsync.factory import logging
 from plextraktsync.plugin import hookimpl
 
 if TYPE_CHECKING:
-    from plextraktsync.config.SyncConfig import SyncConfig
-    from plextraktsync.media.Media import Media
-    from plextraktsync.sync.Sync import Sync
+    from .plugin.SyncPluginInterface import Media, SyncConfig
 
 
 class AddCollectionPlugin:
     logger = logging.getLogger(__name__)
 
     @staticmethod
     def enabled(config: SyncConfig):
         return config.plex_to_trakt["collection"]
 
     @classmethod
-    def factory(cls, sync: Sync):
+    def factory(cls, sync):
         return cls()
 
     @hookimpl
     def walk_movie(self, movie: Media, dry_run: bool):
         self.sync_collection(movie, dry_run=dry_run)
 
     @hookimpl
```

### Comparing `plextraktsync-0.30.0/plextraktsync/sync/ClearCollectedPlugin.py` & `plextraktsync-0.30.1/plextraktsync/sync/ClearCollectedPlugin.py`

 * *Files 19% similar despite different names*

```diff
@@ -3,58 +3,57 @@
 from typing import TYPE_CHECKING, Iterable
 
 from plextraktsync.factory import logging
 from plextraktsync.media.Media import Media
 from plextraktsync.plugin import hookimpl
 
 if TYPE_CHECKING:
-    from plextraktsync.config.SyncConfig import SyncConfig
-    from plextraktsync.sync.Sync import Sync
     from plextraktsync.trakt.TraktApi import TraktApi
     from plextraktsync.trakt.types import TraktMedia
 
+    from .plugin.SyncPluginInterface import Sync, SyncConfig, SyncPluginManager
+
 
 class ClearCollectedPlugin:
     logger = logging.getLogger(__name__)
 
     def __init__(self, trakt: TraktApi):
         self.trakt = trakt
         self.episode_trakt_ids = set()
         self.movie_trakt_ids = set()
-        self.is_partial = None
 
     @staticmethod
     def enabled(config: SyncConfig):
         return config.clear_collected
 
     @classmethod
     def factory(cls, sync: Sync):
         return cls(sync.trakt)
 
     @hookimpl
-    def init(self, is_partial: bool):
-        self.is_partial = is_partial
-        if is_partial:
-            self.logger.warning("Running partial library sync. Clear collected will be disabled.")
+    def init(self, pm: SyncPluginManager, is_partial: bool):
+        if not is_partial:
+            return
+
+        self.logger.warning("Disabling Clear Collected: Running partial library sync")
+        pm.unregister(self)
 
     @hookimpl
     def fini(self, dry_run: bool):
-        if self.is_partial:
-            return
-
         self.clear_collected(self.trakt.movie_collection, self.movie_trakt_ids, dry_run=dry_run)
         self.clear_collected(self.trakt.episodes_collection, self.episode_trakt_ids, dry_run=dry_run)
 
     @hookimpl
     def walk_movie(self, movie: Media):
-        if self.is_partial:
-            return
-
         self.movie_trakt_ids.add(movie.trakt_id)
 
+    @hookimpl
+    def walk_episode(self, episode: Media):
+        self.episode_trakt_ids.add(episode.trakt_id)
+
     def clear_collected(self, existing_items: Iterable[TraktMedia], keep_ids: set[int], dry_run):
         from plextraktsync.trakt.trakt_set import trakt_set
 
         existing_ids = trakt_set(existing_items)
         delete_ids = existing_ids - keep_ids
         delete_items = (tm for tm in existing_items if tm.trakt in delete_ids)
```

### Comparing `plextraktsync-0.30.0/plextraktsync/sync/LikedListsPlugin.py` & `plextraktsync-0.30.1/plextraktsync/sync/TraktListsPlugin.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,36 +1,55 @@
 from __future__ import annotations
 
 from typing import TYPE_CHECKING
 
+from plextraktsync.decorators.measure_time import measure_time
 from plextraktsync.factory import logging
 from plextraktsync.plugin import hookimpl
 
 if TYPE_CHECKING:
-    from plextraktsync.config.SyncConfig import SyncConfig
-    from plextraktsync.sync.Sync import Sync
-    from plextraktsync.trakt.TraktApi import TraktApi
-    from plextraktsync.trakt.TraktUserListCollection import \
-        TraktUserListCollection
+    from .plugin.SyncPluginInterface import Media, Sync, SyncPluginManager
 
 
-class LikedListsPlugin:
+class TraktListsPlugin:
+    """
+    Plugin handling syncing of Trakt lists.
+    """
     logger = logging.getLogger(__name__)
 
-    def __init__(self, trakt: TraktApi):
-        self.trakt = trakt
+    def __init__(self):
+        self.trakt_lists = None
 
     @staticmethod
-    def enabled(config: SyncConfig):
-        return config.sync_liked_lists
+    def enabled(config):
+        # Check for need is performed in init()
+        return True
 
     @classmethod
-    def factory(cls, sync: Sync):
-        return cls(sync.trakt)
+    def factory(cls, sync):
+        return cls()
+
+    @hookimpl(trylast=True)
+    def init(self, pm: SyncPluginManager, sync: Sync):
+        # Skip updating lists if it's empty
+        if sync.trakt_lists.is_empty:
+            self.logger.warning("Disabling TraktListsPlugin: No lists to process")
+            pm.unregister(self)
+            return
+
+        self.trakt_lists = sync.trakt_lists
+
+    @hookimpl
+    def fini(self, dry_run: bool):
+        if dry_run:
+            return
+
+        with measure_time("Updated liked list"):
+            self.trakt_lists.sync()
+
+    @hookimpl
+    def walk_movie(self, movie: Media):
+        self.trakt_lists.add_to_lists(movie)
 
     @hookimpl
-    def init(self, trakt_lists: TraktUserListCollection, is_partial: bool):
-        if is_partial:
-            self.logger.warning("Partial walk, disabling liked lists updating. "
-                                "Liked lists won't update because it needs full library sync.")
-        else:
-            trakt_lists.load_lists(self.trakt.liked_lists)
+    def walk_episode(self, episode: Media):
+        self.trakt_lists.add_to_lists(episode)
```

### Comparing `plextraktsync-0.30.0/plextraktsync/sync/Sync.py` & `plextraktsync-0.30.1/plextraktsync/sync/Sync.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from __future__ import annotations
 
+from functools import cached_property
 from typing import TYPE_CHECKING
 
-from plextraktsync.decorators.measure_time import measure_time
 from plextraktsync.factory import logging
 from plextraktsync.trakt.TraktUserListCollection import TraktUserListCollection
 
 if TYPE_CHECKING:
     from plextraktsync.config.SyncConfig import SyncConfig
     from plextraktsync.plan.Walker import Walker
     from plextraktsync.plex.PlexApi import PlexApi
@@ -18,37 +18,29 @@
 
     def __init__(self, config: SyncConfig, plex: PlexApi, trakt: TraktApi):
         self.config = config
         self.plex = plex
         self.trakt = trakt
         self.walker = None
 
+    @cached_property
+    def trakt_lists(self):
+        return TraktUserListCollection()
+
     def sync(self, walker: Walker, dry_run=False):
         self.walker = walker
-        trakt_lists = TraktUserListCollection()
-        is_partial = walker.is_partial and not dry_run
+        is_partial = walker.is_partial
 
         from plextraktsync.sync.plugin import SyncPluginManager
         pm = SyncPluginManager()
         pm.register_plugins(self)
 
-        pm.hook.init(sync=self, trakt_lists=trakt_lists, is_partial=is_partial, dry_run=dry_run)
-
-        # Skip updating lists if it's empty
-        add_to_lists = not trakt_lists.is_empty
+        pm.hook.init(sync=self, pm=pm, is_partial=is_partial, dry_run=dry_run)
 
         if self.config.need_library_walk:
             for movie in walker.find_movies():
                 pm.hook.walk_movie(movie=movie, dry_run=dry_run)
-                if add_to_lists:
-                    trakt_lists.add_to_lists(movie)
 
             for episode in walker.find_episodes():
                 pm.hook.walk_episode(episode=episode, dry_run=dry_run)
-                if add_to_lists:
-                    trakt_lists.add_to_lists(episode)
-
-        if not dry_run and not trakt_lists.is_empty:
-            with measure_time("Updated liked list"):
-                trakt_lists.sync()
 
-        pm.hook.fini(walker=walker, trakt_lists=trakt_lists, dry_run=dry_run)
+        pm.hook.fini(walker=walker, dry_run=dry_run)
```

### Comparing `plextraktsync-0.30.0/plextraktsync/sync/SyncRatingsPlugin.py` & `plextraktsync-0.30.1/plextraktsync/sync/SyncRatingsPlugin.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,18 +2,15 @@
 
 from typing import TYPE_CHECKING
 
 from plextraktsync.factory import logging
 from plextraktsync.plugin import hookimpl
 
 if TYPE_CHECKING:
-    from plextraktsync.config.SyncConfig import SyncConfig
-    from plextraktsync.media.Media import Media
-    from plextraktsync.plan.Walker import Walker
-    from plextraktsync.sync.Sync import Sync
+    from .plugin.SyncPluginInterface import Media, Sync, SyncConfig, Walker
 
 
 class SyncRatingsPlugin:
     logger = logging.getLogger(__name__)
 
     def __init__(self, config: SyncConfig):
         self.rating_priority = config["rating_priority"]
@@ -26,33 +23,33 @@
         return config.sync_ratings
 
     @classmethod
     def factory(cls, sync: Sync):
         return cls(config=sync.config)
 
     @hookimpl
+    def init(self):
+        self.shows = set()
+
+    @hookimpl
+    def fini(self, walker: Walker, dry_run: bool):
+        for show in walker.walk_shows(self.shows, title="Syncing show ratings"):
+            self.sync_ratings(show, dry_run=dry_run)
+
+    @hookimpl
     def walk_movie(self, movie: Media, dry_run: bool):
         self.sync_ratings(movie, dry_run=dry_run)
 
     @hookimpl
     def walk_episode(self, episode: Media, dry_run: bool):
         self.sync_ratings(episode, dry_run=dry_run)
 
         if episode.show:
             self.shows.add(episode.show)
 
-    @hookimpl
-    def init(self):
-        self.shows = set()
-
-    @hookimpl
-    def fini(self, walker: Walker, dry_run: bool):
-        for show in walker.walk_shows(self.shows, title="Syncing show ratings"):
-            self.sync_ratings(show, dry_run=dry_run)
-
     def sync_ratings(self, m: Media, dry_run: bool):
         if m.plex_rating == m.trakt_rating:
             return
 
         has_trakt = m.trakt_rating is not None
         has_plex = m.plex_rating is not None
         rate = None
```

### Comparing `plextraktsync-0.30.0/plextraktsync/sync/SyncWatchedPlugin.py` & `plextraktsync-0.30.1/plextraktsync/sync/SyncWatchedPlugin.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,17 +2,15 @@
 
 from typing import TYPE_CHECKING
 
 from plextraktsync.factory import logging
 from plextraktsync.plugin import hookimpl
 
 if TYPE_CHECKING:
-    from plextraktsync.config.SyncConfig import SyncConfig
-    from plextraktsync.media.Media import Media
-    from plextraktsync.sync.Sync import Sync
+    from .plugin.SyncPluginInterface import Media, Sync, SyncConfig
 
 
 class SyncWatchedPlugin:
     logger = logging.getLogger(__name__)
 
     def __init__(self, config: SyncConfig):
         self.plex_to_trakt = config.plex_to_trakt["watched_status"]
```

### Comparing `plextraktsync-0.30.0/plextraktsync/sync/WatchListPlugin.py` & `plextraktsync-0.30.1/plextraktsync/sync/WatchListPlugin.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,22 +4,18 @@
 from typing import TYPE_CHECKING
 
 from plextraktsync.decorators.measure_time import measure_time
 from plextraktsync.factory import logging
 from plextraktsync.plugin import hookimpl
 
 if TYPE_CHECKING:
-    from plextraktsync.config.SyncConfig import SyncConfig
-    from plextraktsync.media.Media import Media
-    from plextraktsync.plan.Walker import Walker
     from plextraktsync.plex.PlexApi import PlexApi
-    from plextraktsync.sync.Sync import Sync
     from plextraktsync.trakt.TraktApi import TraktApi
-    from plextraktsync.trakt.TraktUserListCollection import \
-        TraktUserListCollection
+
+    from .plugin.SyncPluginInterface import Media, Sync, SyncConfig, Walker
 
 
 class WatchListPlugin:
     logger = logging.getLogger(__name__)
 
     def __init__(self, config: SyncConfig, plex: PlexApi, trakt: TraktApi):
         self.config = config
@@ -38,21 +34,21 @@
         return cls(
             config=sync.config,
             plex=sync.plex,
             trakt=sync.trakt,
         )
 
     @hookimpl
-    def init(self, trakt_lists: TraktUserListCollection, is_partial: bool):
+    def init(self, sync: Sync, is_partial: bool):
         if self.config.update_plex_wl_as_pl:
             if is_partial:
                 self.logger.warning("Running partial library sync. "
                                     "Watchlist as playlist won't update because it needs full library sync.")
             else:
-                trakt_lists.add_watchlist(self.trakt.watchlist_movies)
+                sync.trakt_lists.add_watchlist(self.trakt.watchlist_movies)
 
     def fini(self, walker: Walker, dry_run: bool):
         if walker.config.walk_watchlist and self.sync_wl:
             with measure_time("Updated watchlist"):
                 self.sync_watchlist(walker, dry_run=dry_run)
 
         if self.config.update_plex_wl_as_pl or self.config.sync_liked_lists:
```

### Comparing `plextraktsync-0.30.0/plextraktsync/sync/WatchProgressPlugin.py` & `plextraktsync-0.30.1/plextraktsync/sync/WatchProgressPlugin.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,18 +4,18 @@
 from typing import TYPE_CHECKING
 
 from plextraktsync.factory import logging
 from plextraktsync.media.Media import Media
 from plextraktsync.plugin import hookimpl
 
 if TYPE_CHECKING:
-    from plextraktsync.config.SyncConfig import SyncConfig
-    from plextraktsync.sync.Sync import Sync
     from plextraktsync.trakt.TraktApi import TraktApi
 
+    from .plugin.SyncPluginInterface import Sync, SyncConfig
+
 
 class WatchProgressPlugin:
     logger = logging.getLogger(__name__)
 
     def __init__(self, trakt: TraktApi):
         self.trakt = trakt
```

### Comparing `plextraktsync-0.30.0/plextraktsync/sync/plugin/SyncPluginManager.py` & `plextraktsync-0.30.1/plextraktsync/sync/plugin/SyncPluginManager.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from __future__ import annotations
 
 from functools import cached_property
 from typing import TYPE_CHECKING
 
 import pluggy
 
+from plextraktsync.decorators.measure_time import measure_time
 from plextraktsync.factory import logging
 
 if TYPE_CHECKING:
     from plextraktsync.sync.Sync import Sync
 
 
 class SyncPluginManager:
@@ -23,31 +24,40 @@
 
         return pm
 
     @cached_property
     def hook(self):
         return self.pm.hook
 
+    @cached_property
+    def unregister(self):
+        return self.pm.unregister
+
     @property
     def plugins(self):
         from ..AddCollectionPlugin import AddCollectionPlugin
         from ..ClearCollectedPlugin import ClearCollectedPlugin
         from ..LikedListsPlugin import LikedListsPlugin
         from ..SyncRatingsPlugin import SyncRatingsPlugin
         from ..SyncWatchedPlugin import SyncWatchedPlugin
+        from ..TraktListsPlugin import TraktListsPlugin
         from ..WatchListPlugin import WatchListPlugin
         from ..WatchProgressPlugin import WatchProgressPlugin
         yield AddCollectionPlugin
         yield ClearCollectedPlugin
         yield LikedListsPlugin
         yield SyncRatingsPlugin
         yield SyncWatchedPlugin
+        yield TraktListsPlugin
         yield WatchListPlugin
         yield WatchProgressPlugin
 
     def register_plugins(self, sync: Sync):
         for plugin in self.plugins:
             enabled = plugin.enabled(sync.config)
             self.logger.info(f"Enable sync plugin '{plugin.__name__}': {enabled}")
             if not enabled:
                 continue
-            self.pm.register(plugin.factory(sync))
+            with measure_time(f"Created '{plugin.__name__}' plugin", logger=self.logger.debug):
+                p = plugin.factory(sync)
+            with measure_time(f"Registered '{plugin.__name__}' plugin", logger=self.logger.debug):
+                self.pm.register(p)
```

### Comparing `plextraktsync-0.30.0/plextraktsync/trakt/ScrobblerCollection.py` & `plextraktsync-0.30.1/plextraktsync/trakt/ScrobblerCollection.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.0/plextraktsync/trakt/ScrobblerProxy.py` & `plextraktsync-0.30.1/plextraktsync/trakt/ScrobblerProxy.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.0/plextraktsync/trakt/TraktApi.py` & `plextraktsync-0.30.1/plextraktsync/trakt/TraktApi.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.0/plextraktsync/trakt/TraktLookup.py` & `plextraktsync-0.30.1/plextraktsync/trakt/TraktLookup.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.0/plextraktsync/trakt/TraktRatingCollection.py` & `plextraktsync-0.30.1/plextraktsync/trakt/TraktRatingCollection.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.0/plextraktsync/trakt/TraktUserList.py` & `plextraktsync-0.30.1/plextraktsync/trakt/TraktUserList.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.0/plextraktsync/trakt/TraktUserListCollection.py` & `plextraktsync-0.30.1/plextraktsync/trakt/TraktUserListCollection.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.0/plextraktsync/trakt/TraktWatchlist.py` & `plextraktsync-0.30.1/plextraktsync/trakt/TraktWatchlist.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.0/plextraktsync/trakt/WatchProgress.py` & `plextraktsync-0.30.1/plextraktsync/trakt/WatchProgress.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.0/plextraktsync/util/Factory.py` & `plextraktsync-0.30.1/plextraktsync/util/Factory.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.0/plextraktsync/util/Path.py` & `plextraktsync-0.30.1/plextraktsync/util/Path.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.0/plextraktsync/util/Rating.py` & `plextraktsync-0.30.1/plextraktsync/util/Rating.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.0/plextraktsync/util/Timer.py` & `plextraktsync-0.30.1/plextraktsync/util/Timer.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.0/plextraktsync/util/Version.py` & `plextraktsync-0.30.1/plextraktsync/util/Version.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.0/plextraktsync/util/local_url.py` & `plextraktsync-0.30.1/plextraktsync/util/local_url.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.0/plextraktsync/util/openurl.py` & `plextraktsync-0.30.1/plextraktsync/util/openurl.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.0/plextraktsync/util/packaging.py` & `plextraktsync-0.30.1/plextraktsync/util/packaging.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.0/plextraktsync/util/remove_empty_values.py` & `plextraktsync-0.30.1/plextraktsync/util/remove_empty_values.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.0/plextraktsync/watch/EventDispatcher.py` & `plextraktsync-0.30.1/plextraktsync/watch/EventDispatcher.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.0/plextraktsync/watch/EventFactory.py` & `plextraktsync-0.30.1/plextraktsync/watch/EventFactory.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.0/plextraktsync/watch/ProgressBar.py` & `plextraktsync-0.30.1/plextraktsync/watch/ProgressBar.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.0/plextraktsync/watch/WatchStateUpdater.py` & `plextraktsync-0.30.1/plextraktsync/watch/WatchStateUpdater.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.0/plextraktsync/watch/WebSocketListener.py` & `plextraktsync-0.30.1/plextraktsync/watch/WebSocketListener.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.0/plextraktsync/watch/events.py` & `plextraktsync-0.30.1/plextraktsync/watch/events.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.0/requirements.txt` & `plextraktsync-0.30.1/requirements.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 attrs==23.2.0; python_version >= '3.7'
 cattrs==23.2.3; python_version >= '3.7' and python_version >= '3.8'
 certifi==2024.2.2; python_version >= '3.6'
 charset-normalizer==3.3.2; python_full_version >= '3.7.0'
 click==8.1.7; python_version >= '3.7'
 deprecated==1.2.14; python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'
-exceptiongroup==1.2.0; python_version < '3.11'
+exceptiongroup==1.2.1; python_version >= '3.7'
 humanize==4.9.0; python_version >= '3.8'
 idna==3.7; python_version >= '3.5'
 inquirerpy==0.3.4; python_version >= '3.7' and python_version < '4.0'
 markdown-it-py==3.0.0; python_version >= '3.7' and python_version >= '3.8'
 mdurl==0.1.2; python_version >= '3.7'
 oauthlib==3.2.2; python_version >= '3.6'
 pfzy==0.3.4; python_version >= '3.7' and python_version < '4.0'
-platformdirs==4.2.0; python_version >= '3.7' and python_version >= '3.8'
-plexapi==4.15.11; python_version >= '3.8'
-pluggy==1.4.0; python_version >= '3.8'
+platformdirs==4.2.1; python_version >= '3.8'
+plexapi==4.15.12; python_version >= '3.8'
+pluggy==1.5.0; python_version >= '3.8'
 prompt-toolkit==3.0.43; python_full_version >= '3.7.0'
 pygments==2.17.2; python_version >= '3.7'
 python-dotenv==1.0.1; python_version >= '3.8'
 python-git-info==0.8.3
 pytimeparse==1.1.8
 pytrakt==3.4.32
 pyyaml==6.0.1; python_version >= '3.6'
@@ -28,9 +28,9 @@
 rich==13.7.1; python_full_version >= '3.7.0'
 six==1.16.0; python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3' and python_version >= '3.4'
 tqdm==4.66.2; python_version >= '3.7'
 typing-extensions==4.11.0; python_version < '3.11'
 url-normalize==1.4.3; python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4, 3.5' and python_version >= '3.6'
 urllib3==2.2.1; python_version >= '3.8'
 wcwidth==0.2.13
-websocket-client==1.7.0; python_version >= '3.8'
+websocket-client==1.8.0; python_version >= '3.8'
 wrapt==1.16.0; python_version >= '3.5' and python_version >= '3.6'
```

### Comparing `plextraktsync-0.30.0/setup.cfg` & `plextraktsync-0.30.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.0/tests/test_collection_metadata.py` & `plextraktsync-0.30.1/tests/test_collection_metadata.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.0/tests/test_config.py` & `plextraktsync-0.30.1/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.0/tests/test_events.py` & `plextraktsync-0.30.1/tests/test_events.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.0/tests/test_new_agent.py` & `plextraktsync-0.30.1/tests/test_new_agent.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.0/tests/test_plex_id.py` & `plextraktsync-0.30.1/tests/test_plex_id.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.0/tests/test_rating.py` & `plextraktsync-0.30.1/tests/test_rating.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.0/tests/test_timer.py` & `plextraktsync-0.30.1/tests/test_timer.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.0/tests/test_trakt_progress.py` & `plextraktsync-0.30.1/tests/test_trakt_progress.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.0/tests/test_tv_lookup.py` & `plextraktsync-0.30.1/tests/test_tv_lookup.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.0/tests/test_walker.py` & `plextraktsync-0.30.1/tests/test_walker.py`

 * *Files identical despite different names*

