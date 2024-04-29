# Comparing `tmp/troi-2024.4.26.0.tar.gz` & `tmp/troi-29.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "troi-2024.4.26.0.tar", last modified: Fri Apr 26 10:21:36 2024, max compression
+gzip compressed data, was "troi-29.0.tar", last modified: Mon Apr 29 12:03:53 2024, max compression
```

## Comparing `troi-2024.4.26.0.tar` & `troi-29.0.tar`

### file list

```diff
@@ -1,161 +1,161 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:21:36.264179 troi-2024.4.26.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:21:36.236178 troi-2024.4.26.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:21:36.240178 troi-2024.4.26.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      583 2024-04-26 10:21:02.000000 troi-2024.4.26.0/.github/workflows/cd.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1656 2024-04-26 10:21:02.000000 troi-2024.4.26.0/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-26 10:21:02.000000 troi-2024.4.26.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-26 10:21:02.000000 troi-2024.4.26.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    18092 2024-04-26 10:21:02.000000 troi-2024.4.26.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     7784 2024-04-26 10:21:36.264179 troi-2024.4.26.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5832 2024-04-26 10:21:02.000000 troi-2024.4.26.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      422 2024-04-26 10:21:02.000000 troi-2024.4.26.0/config.py.sample
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:21:36.240178 troi-2024.4.26.0/docker/
--rwxr-xr-x   0 runner    (1001) docker     (127)       54 2024-04-26 10:21:02.000000 troi-2024.4.26.0/docker/endless.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:21:36.244179 troi-2024.4.26.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-26 10:21:02.000000 troi-2024.4.26.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     3055 2024-04-26 10:21:02.000000 troi-2024.4.26.0/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:21:36.244179 troi-2024.4.26.0/docs/dev/
--rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-04-26 10:21:02.000000 troi-2024.4.26.0/docs/dev/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:21:36.244179 troi-2024.4.26.0/docs/elements/
--rw-r--r--   0 runner    (1001) docker     (127)     1311 2024-04-26 10:21:02.000000 troi-2024.4.26.0/docs/elements/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3453 2024-04-26 10:21:02.000000 troi-2024.4.26.0/docs/elements/listenbrainz.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-04-26 10:21:02.000000 troi-2024.4.26.0/docs/elements/musicbrainz.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-04-26 10:21:02.000000 troi-2024.4.26.0/docs/entities.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3363 2024-04-26 10:21:02.000000 troi-2024.4.26.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      730 2024-04-26 10:21:02.000000 troi-2024.4.26.0/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2927 2024-04-26 10:21:02.000000 troi-2024.4.26.0/docs/introduction.rst
--rw-r--r--   0 runner    (1001) docker     (127)     9372 2024-04-26 10:21:02.000000 troi-2024.4.26.0/docs/lb_radio.rst
--rw-r--r--   0 runner    (1001) docker     (127)    19960 2024-04-26 10:21:02.000000 troi-2024.4.26.0/docs/listenbrainz-logo.svg
--rw-r--r--   0 runner    (1001) docker     (127)      795 2024-04-26 10:21:02.000000 troi-2024.4.26.0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)     1647 2024-04-26 10:21:02.000000 troi-2024.4.26.0/docs/patches.rst
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-26 10:21:02.000000 troi-2024.4.26.0/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      560 2024-04-26 10:21:02.000000 troi-2024.4.26.0/docs/troi-arguments.rst
--rw-r--r--   0 runner    (1001) docker     (127)     7903 2024-04-26 10:21:02.000000 troi-2024.4.26.0/docs/user-guide.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1691 2024-04-26 10:21:02.000000 troi-2024.4.26.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 10:21:36.264179 troi-2024.4.26.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:21:36.248179 troi-2024.4.26.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 10:21:02.000000 troi-2024.4.26.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:21:36.248179 troi-2024.4.26.0/tests/listenbrainz/
--rw-r--r--   0 runner    (1001) docker     (127)     1638 2024-04-26 10:21:02.000000 troi-2024.4.26.0/tests/listenbrainz/test_recs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2980 2024-04-26 10:21:02.000000 troi-2024.4.26.0/tests/listenbrainz/test_stats.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:21:36.248179 troi-2024.4.26.0/tests/musicbrainz/
--rw-r--r--   0 runner    (1001) docker     (127)     2519 2024-04-26 10:21:02.000000 troi-2024.4.26.0/tests/musicbrainz/test_mbid_mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)    14691 2024-04-26 10:21:02.000000 troi-2024.4.26.0/tests/musicbrainz/test_recording_lookup.py
--rw-r--r--   0 runner    (1001) docker     (127)     2259 2024-04-26 10:21:02.000000 troi-2024.4.26.0/tests/musicbrainz/test_related_artist_credits.py
--rw-r--r--   0 runner    (1001) docker     (127)     3759 2024-04-26 10:21:02.000000 troi-2024.4.26.0/tests/test_entities.py
--rw-r--r--   0 runner    (1001) docker     (127)    11684 2024-04-26 10:21:02.000000 troi-2024.4.26.0/tests/test_filters.py
--rw-r--r--   0 runner    (1001) docker     (127)     8199 2024-04-26 10:21:02.000000 troi-2024.4.26.0/tests/test_operations.py
--rw-r--r--   0 runner    (1001) docker     (127)     8646 2024-04-26 10:21:02.000000 troi-2024.4.26.0/tests/test_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     7819 2024-04-26 10:21:02.000000 troi-2024.4.26.0/tests/test_playlist.py
--rw-r--r--   0 runner    (1001) docker     (127)      648 2024-04-26 10:21:02.000000 troi-2024.4.26.0/tests/test_plist.py
--rw-r--r--   0 runner    (1001) docker     (127)     1279 2024-04-26 10:21:02.000000 troi-2024.4.26.0/tests/test_sorts.py
--rw-r--r--   0 runner    (1001) docker     (127)      627 2024-04-26 10:21:02.000000 troi-2024.4.26.0/tests/test_tag_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      459 2024-04-26 10:21:02.000000 troi-2024.4.26.0/tests/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:21:36.248179 troi-2024.4.26.0/tests/tools/
--rw-r--r--   0 runner    (1001) docker     (127)      789 2024-04-26 10:21:02.000000 troi-2024.4.26.0/tests/tools/test_area_lookup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:21:36.252179 troi-2024.4.26.0/troi/
--rw-r--r--   0 runner    (1001) docker     (127)    13635 2024-04-26 10:21:02.000000 troi-2024.4.26.0/troi/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     9616 2024-04-26 10:21:02.000000 troi-2024.4.26.0/troi/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:21:36.252179 troi-2024.4.26.0/troi/content_resolver/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:21:02.000000 troi-2024.4.26.0/troi/content_resolver/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4411 2024-04-26 10:21:02.000000 troi-2024.4.26.0/troi/content_resolver/artist_search.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     8637 2024-04-26 10:21:02.000000 troi-2024.4.26.0/troi/content_resolver/cli.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     9460 2024-04-26 10:21:02.000000 troi-2024.4.26.0/troi/content_resolver/content_resolver.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    18059 2024-04-26 10:21:02.000000 troi-2024.4.26.0/troi/content_resolver/database.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3647 2024-04-26 10:21:02.000000 troi-2024.4.26.0/troi/content_resolver/duplicates.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:21:36.256178 troi-2024.4.26.0/troi/content_resolver/formats/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:21:02.000000 troi-2024.4.26.0/troi/content_resolver/formats/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      899 2024-04-26 10:21:02.000000 troi-2024.4.26.0/troi/content_resolver/formats/flac.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1189 2024-04-26 10:21:02.000000 troi-2024.4.26.0/troi/content_resolver/formats/m4a.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1977 2024-04-26 10:21:02.000000 troi-2024.4.26.0/troi/content_resolver/formats/mp3.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      913 2024-04-26 10:21:02.000000 troi-2024.4.26.0/troi/content_resolver/formats/ogg_opus.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      903 2024-04-26 10:21:02.000000 troi-2024.4.26.0/troi/content_resolver/formats/ogg_vorbis.py
--rw-r--r--   0 runner    (1001) docker     (127)     1185 2024-04-26 10:21:02.000000 troi-2024.4.26.0/troi/content_resolver/formats/tag_utils.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      968 2024-04-26 10:21:02.000000 troi-2024.4.26.0/troi/content_resolver/formats/wma.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3345 2024-04-26 10:21:02.000000 troi-2024.4.26.0/troi/content_resolver/fuzzy_index.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2677 2024-04-26 10:21:02.000000 troi-2024.4.26.0/troi/content_resolver/lb_radio.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6199 2024-04-26 10:21:02.000000 troi-2024.4.26.0/troi/content_resolver/metadata_lookup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:21:36.256178 troi-2024.4.26.0/troi/content_resolver/model/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 10:21:02.000000 troi-2024.4.26.0/troi/content_resolver/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-04-26 10:21:02.000000 troi-2024.4.26.0/troi/content_resolver/model/database.py
--rw-r--r--   0 runner    (1001) docker     (127)      409 2024-04-26 10:21:02.000000 troi-2024.4.26.0/troi/content_resolver/model/directory.py
--rw-r--r--   0 runner    (1001) docker     (127)     2186 2024-04-26 10:21:02.000000 troi-2024.4.26.0/troi/content_resolver/model/recording.py
--rw-r--r--   0 runner    (1001) docker     (127)      918 2024-04-26 10:21:02.000000 troi-2024.4.26.0/troi/content_resolver/model/tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      858 2024-04-26 10:21:02.000000 troi-2024.4.26.0/troi/content_resolver/model/unresolved_recording.py
--rw-r--r--   0 runner    (1001) docker     (127)     1271 2024-04-26 10:21:02.000000 troi-2024.4.26.0/troi/content_resolver/playlist.py
--rw-r--r--   0 runner    (1001) docker     (127)      725 2024-04-26 10:21:02.000000 troi-2024.4.26.0/troi/content_resolver/py_sonic_fix.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    10148 2024-04-26 10:21:02.000000 troi-2024.4.26.0/troi/content_resolver/subsonic.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5400 2024-04-26 10:21:02.000000 troi-2024.4.26.0/troi/content_resolver/tag_search.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1230 2024-04-26 10:21:02.000000 troi-2024.4.26.0/troi/content_resolver/top_tags.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6273 2024-04-26 10:21:02.000000 troi-2024.4.26.0/troi/content_resolver/unresolved_recording.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3457 2024-04-26 10:21:02.000000 troi-2024.4.26.0/troi/content_resolver/utils.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1714 2024-04-26 10:21:02.000000 troi-2024.4.26.0/troi/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:21:36.256178 troi-2024.4.26.0/troi/external/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 10:21:02.000000 troi-2024.4.26.0/troi/external/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2281 2024-04-26 10:21:02.000000 troi-2024.4.26.0/troi/external/gpt.py
--rw-r--r--   0 runner    (1001) docker     (127)    12835 2024-04-26 10:21:02.000000 troi-2024.4.26.0/troi/filters.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:21:36.256178 troi-2024.4.26.0/troi/listenbrainz/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 10:21:02.000000 troi-2024.4.26.0/troi/listenbrainz/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1996 2024-04-26 10:21:02.000000 troi-2024.4.26.0/troi/listenbrainz/feedback.py
--rw-r--r--   0 runner    (1001) docker     (127)     4093 2024-04-26 10:21:02.000000 troi-2024.4.26.0/troi/listenbrainz/listens.py
--rw-r--r--   0 runner    (1001) docker     (127)     3019 2024-04-26 10:21:02.000000 troi-2024.4.26.0/troi/listenbrainz/recs.py
--rw-r--r--   0 runner    (1001) docker     (127)     4449 2024-04-26 10:21:02.000000 troi-2024.4.26.0/troi/listenbrainz/stats.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:21:36.260179 troi-2024.4.26.0/troi/listenbrainz/unused/
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-26 10:21:02.000000 troi-2024.4.26.0/troi/listenbrainz/unused/README.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2737 2024-04-26 10:21:02.000000 troi-2024.4.26.0/troi/listenbrainz/unused/dataset_fetcher.py
--rw-r--r--   0 runner    (1001) docker     (127)      529 2024-04-26 10:21:02.000000 troi-2024.4.26.0/troi/listenbrainz/user.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:21:36.260179 troi-2024.4.26.0/troi/local/
--rwxr-xr-x   0 runner    (1001) docker     (127)     1388 2024-04-26 10:21:02.000000 troi-2024.4.26.0/troi/local/periodic_jams_local.py
--rw-r--r--   0 runner    (1001) docker     (127)     3369 2024-04-26 10:21:02.000000 troi-2024.4.26.0/troi/local/recording_resolver.py
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-26 10:21:02.000000 troi-2024.4.26.0/troi/logging_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3521 2024-04-26 10:21:02.000000 troi-2024.4.26.0/troi/loops.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:21:36.260179 troi-2024.4.26.0/troi/musicbrainz/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 10:21:02.000000 troi-2024.4.26.0/troi/musicbrainz/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2096 2024-04-26 10:21:02.000000 troi-2024.4.26.0/troi/musicbrainz/mbid_mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)      833 2024-04-26 10:21:02.000000 troi-2024.4.26.0/troi/musicbrainz/mbid_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)      530 2024-04-26 10:21:02.000000 troi-2024.4.26.0/troi/musicbrainz/recording.py
--rw-r--r--   0 runner    (1001) docker     (127)     5685 2024-04-26 10:21:02.000000 troi-2024.4.26.0/troi/musicbrainz/recording_lookup.py
--rw-r--r--   0 runner    (1001) docker     (127)     1565 2024-04-26 10:21:02.000000 troi-2024.4.26.0/troi/musicbrainz/related_artist_credits.py
--rw-r--r--   0 runner    (1001) docker     (127)     6309 2024-04-26 10:21:02.000000 troi-2024.4.26.0/troi/operations.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6070 2024-04-26 10:21:02.000000 troi-2024.4.26.0/troi/parse_prompt.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     8787 2024-04-26 10:21:02.000000 troi-2024.4.26.0/troi/patch.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:21:36.260179 troi-2024.4.26.0/troi/patches/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 10:21:02.000000 troi-2024.4.26.0/troi/patches/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1442 2024-04-26 10:21:02.000000 troi-2024.4.26.0/troi/patches/ai_jams.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    10520 2024-04-26 10:21:02.000000 troi-2024.4.26.0/troi/patches/lb_radio.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:21:36.264179 troi-2024.4.26.0/troi/patches/lb_radio_classes/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 10:21:02.000000 troi-2024.4.26.0/troi/patches/lb_radio_classes/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3041 2024-04-26 10:21:02.000000 troi-2024.4.26.0/troi/patches/lb_radio_classes/artist.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3457 2024-04-26 10:21:02.000000 troi-2024.4.26.0/troi/patches/lb_radio_classes/blend.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1643 2024-04-26 10:21:02.000000 troi-2024.4.26.0/troi/patches/lb_radio_classes/collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     4034 2024-04-26 10:21:02.000000 troi-2024.4.26.0/troi/patches/lb_radio_classes/country.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1543 2024-04-26 10:21:02.000000 troi-2024.4.26.0/troi/patches/lb_radio_classes/playlist.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2880 2024-04-26 10:21:02.000000 troi-2024.4.26.0/troi/patches/lb_radio_classes/recs.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2850 2024-04-26 10:21:02.000000 troi-2024.4.26.0/troi/patches/lb_radio_classes/stats.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4118 2024-04-26 10:21:02.000000 troi-2024.4.26.0/troi/patches/lb_radio_classes/tag.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6880 2024-04-26 10:21:02.000000 troi-2024.4.26.0/troi/patches/periodic_jams.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3150 2024-04-26 10:21:02.000000 troi-2024.4.26.0/troi/patches/periodic_jams_local.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2022 2024-04-26 10:21:02.000000 troi-2024.4.26.0/troi/patches/playlist_from_listenbrainz.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1180 2024-04-26 10:21:02.000000 troi-2024.4.26.0/troi/patches/playlist_from_mbids.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3878 2024-04-26 10:21:02.000000 troi-2024.4.26.0/troi/patches/recs_to_playlist.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:21:36.264179 troi-2024.4.26.0/troi/patches/unused/
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-26 10:21:02.000000 troi-2024.4.26.0/troi/patches/unused/README.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)     2550 2024-04-26 10:21:02.000000 troi-2024.4.26.0/troi/patches/unused/area_random_recordings.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    20763 2024-04-26 10:21:02.000000 troi-2024.4.26.0/troi/playlist.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2747 2024-04-26 10:21:02.000000 troi-2024.4.26.0/troi/plist.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4866 2024-04-26 10:21:02.000000 troi-2024.4.26.0/troi/print_recording.py
--rw-r--r--   0 runner    (1001) docker     (127)     3342 2024-04-26 10:21:02.000000 troi-2024.4.26.0/troi/recording_search_service.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      682 2024-04-26 10:21:02.000000 troi-2024.4.26.0/troi/service.py
--rw-r--r--   0 runner    (1001) docker     (127)      954 2024-04-26 10:21:02.000000 troi-2024.4.26.0/troi/sorts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:21:36.264179 troi-2024.4.26.0/troi/tools/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 10:21:02.000000 troi-2024.4.26.0/troi/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      810 2024-04-26 10:21:02.000000 troi-2024.4.26.0/troi/tools/area_lookup.py
--rw-r--r--   0 runner    (1001) docker     (127)     7005 2024-04-26 10:21:02.000000 troi-2024.4.26.0/troi/tools/spotify_lookup.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2912 2024-04-26 10:21:02.000000 troi-2024.4.26.0/troi/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:21:36.264179 troi-2024.4.26.0/troi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7784 2024-04-26 10:21:36.000000 troi-2024.4.26.0/troi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3873 2024-04-26 10:21:36.000000 troi-2024.4.26.0/troi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 10:21:36.000000 troi-2024.4.26.0/troi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 10:21:36.000000 troi-2024.4.26.0/troi.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      527 2024-04-26 10:21:36.000000 troi-2024.4.26.0/troi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-26 10:21:36.000000 troi-2024.4.26.0/troi.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:03:53.787052 troi-29.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:03:53.759052 troi-29.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:03:53.763052 troi-29.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      583 2024-04-29 12:03:22.000000 troi-29.0/.github/workflows/cd.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1656 2024-04-29 12:03:22.000000 troi-29.0/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-29 12:03:22.000000 troi-29.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-29 12:03:22.000000 troi-29.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    18092 2024-04-29 12:03:22.000000 troi-29.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7777 2024-04-29 12:03:53.787052 troi-29.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5832 2024-04-29 12:03:22.000000 troi-29.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      422 2024-04-29 12:03:22.000000 troi-29.0/config.py.sample
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:03:53.763052 troi-29.0/docker/
+-rwxr-xr-x   0 runner    (1001) docker     (127)       54 2024-04-29 12:03:22.000000 troi-29.0/docker/endless.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:03:53.767052 troi-29.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-29 12:03:22.000000 troi-29.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     3055 2024-04-29 12:03:22.000000 troi-29.0/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:03:53.767052 troi-29.0/docs/dev/
+-rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-04-29 12:03:22.000000 troi-29.0/docs/dev/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:03:53.767052 troi-29.0/docs/elements/
+-rw-r--r--   0 runner    (1001) docker     (127)     1311 2024-04-29 12:03:22.000000 troi-29.0/docs/elements/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3453 2024-04-29 12:03:22.000000 troi-29.0/docs/elements/listenbrainz.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-04-29 12:03:22.000000 troi-29.0/docs/elements/musicbrainz.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-04-29 12:03:22.000000 troi-29.0/docs/entities.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3363 2024-04-29 12:03:22.000000 troi-29.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      730 2024-04-29 12:03:22.000000 troi-29.0/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2927 2024-04-29 12:03:22.000000 troi-29.0/docs/introduction.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     9372 2024-04-29 12:03:22.000000 troi-29.0/docs/lb_radio.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    19960 2024-04-29 12:03:22.000000 troi-29.0/docs/listenbrainz-logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      795 2024-04-29 12:03:22.000000 troi-29.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)     1647 2024-04-29 12:03:22.000000 troi-29.0/docs/patches.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-29 12:03:22.000000 troi-29.0/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      560 2024-04-29 12:03:22.000000 troi-29.0/docs/troi-arguments.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7903 2024-04-29 12:03:22.000000 troi-29.0/docs/user-guide.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1691 2024-04-29 12:03:22.000000 troi-29.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 12:03:53.787052 troi-29.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:03:53.767052 troi-29.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 12:03:22.000000 troi-29.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:03:53.771052 troi-29.0/tests/listenbrainz/
+-rw-r--r--   0 runner    (1001) docker     (127)     1638 2024-04-29 12:03:22.000000 troi-29.0/tests/listenbrainz/test_recs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2980 2024-04-29 12:03:22.000000 troi-29.0/tests/listenbrainz/test_stats.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:03:53.771052 troi-29.0/tests/musicbrainz/
+-rw-r--r--   0 runner    (1001) docker     (127)     2519 2024-04-29 12:03:22.000000 troi-29.0/tests/musicbrainz/test_mbid_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14691 2024-04-29 12:03:22.000000 troi-29.0/tests/musicbrainz/test_recording_lookup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2259 2024-04-29 12:03:22.000000 troi-29.0/tests/musicbrainz/test_related_artist_credits.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3759 2024-04-29 12:03:22.000000 troi-29.0/tests/test_entities.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11684 2024-04-29 12:03:22.000000 troi-29.0/tests/test_filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8199 2024-04-29 12:03:22.000000 troi-29.0/tests/test_operations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8646 2024-04-29 12:03:22.000000 troi-29.0/tests/test_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7819 2024-04-29 12:03:22.000000 troi-29.0/tests/test_playlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)      648 2024-04-29 12:03:22.000000 troi-29.0/tests/test_plist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1279 2024-04-29 12:03:22.000000 troi-29.0/tests/test_sorts.py
+-rw-r--r--   0 runner    (1001) docker     (127)      627 2024-04-29 12:03:22.000000 troi-29.0/tests/test_tag_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2024-04-29 12:03:22.000000 troi-29.0/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:03:53.771052 troi-29.0/tests/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)      789 2024-04-29 12:03:22.000000 troi-29.0/tests/tools/test_area_lookup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:03:53.771052 troi-29.0/troi/
+-rw-r--r--   0 runner    (1001) docker     (127)    13635 2024-04-29 12:03:22.000000 troi-29.0/troi/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9616 2024-04-29 12:03:22.000000 troi-29.0/troi/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:03:53.775052 troi-29.0/troi/content_resolver/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:03:22.000000 troi-29.0/troi/content_resolver/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4411 2024-04-29 12:03:22.000000 troi-29.0/troi/content_resolver/artist_search.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8637 2024-04-29 12:03:22.000000 troi-29.0/troi/content_resolver/cli.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9460 2024-04-29 12:03:22.000000 troi-29.0/troi/content_resolver/content_resolver.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    18059 2024-04-29 12:03:22.000000 troi-29.0/troi/content_resolver/database.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3647 2024-04-29 12:03:22.000000 troi-29.0/troi/content_resolver/duplicates.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:03:53.775052 troi-29.0/troi/content_resolver/formats/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:03:22.000000 troi-29.0/troi/content_resolver/formats/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      899 2024-04-29 12:03:22.000000 troi-29.0/troi/content_resolver/formats/flac.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1189 2024-04-29 12:03:22.000000 troi-29.0/troi/content_resolver/formats/m4a.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1977 2024-04-29 12:03:22.000000 troi-29.0/troi/content_resolver/formats/mp3.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      913 2024-04-29 12:03:22.000000 troi-29.0/troi/content_resolver/formats/ogg_opus.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      903 2024-04-29 12:03:22.000000 troi-29.0/troi/content_resolver/formats/ogg_vorbis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1185 2024-04-29 12:03:22.000000 troi-29.0/troi/content_resolver/formats/tag_utils.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      968 2024-04-29 12:03:22.000000 troi-29.0/troi/content_resolver/formats/wma.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3345 2024-04-29 12:03:22.000000 troi-29.0/troi/content_resolver/fuzzy_index.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2677 2024-04-29 12:03:22.000000 troi-29.0/troi/content_resolver/lb_radio.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6199 2024-04-29 12:03:22.000000 troi-29.0/troi/content_resolver/metadata_lookup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:03:53.779052 troi-29.0/troi/content_resolver/model/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 12:03:22.000000 troi-29.0/troi/content_resolver/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-04-29 12:03:22.000000 troi-29.0/troi/content_resolver/model/database.py
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2024-04-29 12:03:22.000000 troi-29.0/troi/content_resolver/model/directory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2186 2024-04-29 12:03:22.000000 troi-29.0/troi/content_resolver/model/recording.py
+-rw-r--r--   0 runner    (1001) docker     (127)      918 2024-04-29 12:03:22.000000 troi-29.0/troi/content_resolver/model/tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      858 2024-04-29 12:03:22.000000 troi-29.0/troi/content_resolver/model/unresolved_recording.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1271 2024-04-29 12:03:22.000000 troi-29.0/troi/content_resolver/playlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)      725 2024-04-29 12:03:22.000000 troi-29.0/troi/content_resolver/py_sonic_fix.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    10148 2024-04-29 12:03:22.000000 troi-29.0/troi/content_resolver/subsonic.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5400 2024-04-29 12:03:22.000000 troi-29.0/troi/content_resolver/tag_search.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1230 2024-04-29 12:03:22.000000 troi-29.0/troi/content_resolver/top_tags.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6273 2024-04-29 12:03:22.000000 troi-29.0/troi/content_resolver/unresolved_recording.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3457 2024-04-29 12:03:22.000000 troi-29.0/troi/content_resolver/utils.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1714 2024-04-29 12:03:22.000000 troi-29.0/troi/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:03:53.779052 troi-29.0/troi/external/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 12:03:22.000000 troi-29.0/troi/external/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2281 2024-04-29 12:03:22.000000 troi-29.0/troi/external/gpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12835 2024-04-29 12:03:22.000000 troi-29.0/troi/filters.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:03:53.779052 troi-29.0/troi/listenbrainz/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 12:03:22.000000 troi-29.0/troi/listenbrainz/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1996 2024-04-29 12:03:22.000000 troi-29.0/troi/listenbrainz/feedback.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4093 2024-04-29 12:03:22.000000 troi-29.0/troi/listenbrainz/listens.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3019 2024-04-29 12:03:22.000000 troi-29.0/troi/listenbrainz/recs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4449 2024-04-29 12:03:22.000000 troi-29.0/troi/listenbrainz/stats.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:03:53.779052 troi-29.0/troi/listenbrainz/unused/
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-29 12:03:22.000000 troi-29.0/troi/listenbrainz/unused/README.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2737 2024-04-29 12:03:22.000000 troi-29.0/troi/listenbrainz/unused/dataset_fetcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)      529 2024-04-29 12:03:22.000000 troi-29.0/troi/listenbrainz/user.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:03:53.779052 troi-29.0/troi/local/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1388 2024-04-29 12:03:22.000000 troi-29.0/troi/local/periodic_jams_local.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3369 2024-04-29 12:03:22.000000 troi-29.0/troi/local/recording_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-29 12:03:22.000000 troi-29.0/troi/logging_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3521 2024-04-29 12:03:22.000000 troi-29.0/troi/loops.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:03:53.779052 troi-29.0/troi/musicbrainz/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 12:03:22.000000 troi-29.0/troi/musicbrainz/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2096 2024-04-29 12:03:22.000000 troi-29.0/troi/musicbrainz/mbid_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)      833 2024-04-29 12:03:22.000000 troi-29.0/troi/musicbrainz/mbid_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)      530 2024-04-29 12:03:22.000000 troi-29.0/troi/musicbrainz/recording.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5685 2024-04-29 12:03:22.000000 troi-29.0/troi/musicbrainz/recording_lookup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1565 2024-04-29 12:03:22.000000 troi-29.0/troi/musicbrainz/related_artist_credits.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6309 2024-04-29 12:03:22.000000 troi-29.0/troi/operations.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6070 2024-04-29 12:03:22.000000 troi-29.0/troi/parse_prompt.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8787 2024-04-29 12:03:22.000000 troi-29.0/troi/patch.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:03:53.783052 troi-29.0/troi/patches/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 12:03:22.000000 troi-29.0/troi/patches/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1442 2024-04-29 12:03:22.000000 troi-29.0/troi/patches/ai_jams.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    10520 2024-04-29 12:03:22.000000 troi-29.0/troi/patches/lb_radio.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:03:53.783052 troi-29.0/troi/patches/lb_radio_classes/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 12:03:22.000000 troi-29.0/troi/patches/lb_radio_classes/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3041 2024-04-29 12:03:22.000000 troi-29.0/troi/patches/lb_radio_classes/artist.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3457 2024-04-29 12:03:22.000000 troi-29.0/troi/patches/lb_radio_classes/blend.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1643 2024-04-29 12:03:22.000000 troi-29.0/troi/patches/lb_radio_classes/collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4034 2024-04-29 12:03:22.000000 troi-29.0/troi/patches/lb_radio_classes/country.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1544 2024-04-29 12:03:22.000000 troi-29.0/troi/patches/lb_radio_classes/playlist.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2880 2024-04-29 12:03:22.000000 troi-29.0/troi/patches/lb_radio_classes/recs.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2850 2024-04-29 12:03:22.000000 troi-29.0/troi/patches/lb_radio_classes/stats.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4118 2024-04-29 12:03:22.000000 troi-29.0/troi/patches/lb_radio_classes/tag.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6880 2024-04-29 12:03:22.000000 troi-29.0/troi/patches/periodic_jams.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3116 2024-04-29 12:03:22.000000 troi-29.0/troi/patches/periodic_jams_local.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1981 2024-04-29 12:03:22.000000 troi-29.0/troi/patches/playlist_from_listenbrainz.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1183 2024-04-29 12:03:22.000000 troi-29.0/troi/patches/playlist_from_mbids.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3881 2024-04-29 12:03:22.000000 troi-29.0/troi/patches/recs_to_playlist.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:03:53.783052 troi-29.0/troi/patches/unused/
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-29 12:03:22.000000 troi-29.0/troi/patches/unused/README.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2550 2024-04-29 12:03:22.000000 troi-29.0/troi/patches/unused/area_random_recordings.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    20763 2024-04-29 12:03:22.000000 troi-29.0/troi/playlist.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2747 2024-04-29 12:03:22.000000 troi-29.0/troi/plist.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4866 2024-04-29 12:03:22.000000 troi-29.0/troi/print_recording.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3342 2024-04-29 12:03:22.000000 troi-29.0/troi/recording_search_service.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      682 2024-04-29 12:03:22.000000 troi-29.0/troi/service.py
+-rw-r--r--   0 runner    (1001) docker     (127)      954 2024-04-29 12:03:22.000000 troi-29.0/troi/sorts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:03:53.783052 troi-29.0/troi/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 12:03:22.000000 troi-29.0/troi/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      810 2024-04-29 12:03:22.000000 troi-29.0/troi/tools/area_lookup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7005 2024-04-29 12:03:22.000000 troi-29.0/troi/tools/spotify_lookup.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2912 2024-04-29 12:03:22.000000 troi-29.0/troi/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:03:53.783052 troi-29.0/troi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7777 2024-04-29 12:03:53.000000 troi-29.0/troi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3873 2024-04-29 12:03:53.000000 troi-29.0/troi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 12:03:53.000000 troi-29.0/troi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 12:03:53.000000 troi-29.0/troi.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      527 2024-04-29 12:03:53.000000 troi-29.0/troi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-29 12:03:53.000000 troi-29.0/troi.egg-info/top_level.txt
```

### Comparing `troi-2024.4.26.0/.github/workflows/cd.yml` & `troi-29.0/.github/workflows/cd.yml`

 * *Files identical despite different names*

### Comparing `troi-2024.4.26.0/.github/workflows/ci.yml` & `troi-29.0/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `troi-2024.4.26.0/LICENSE` & `troi-29.0/LICENSE`

 * *Files identical despite different names*

### Comparing `troi-2024.4.26.0/PKG-INFO` & `troi-29.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: troi
-Version: 2024.4.26.0
+Version: 29.0
 Summary: ListenBrainz' empathic music recommendation/playlisting engine
 Author-email: MetaBrainz Foundation <support@metabrainz.org>
 Project-URL: Homepage, https://github.com/metabrainz/troi-recommendation-playground
 Project-URL: Documentation, https://troi.readthedocs.io/en/latest/
 Project-URL: Releases, https://github.com/metabrainz/troi-recommendation-playground/releases
 Project-URL: Issues, https://tickets.metabrainz.org/secure/RapidBoard.jspa?rapidView=14&projectKey=LB#
 Classifier: Programming Language :: Python :: 3
```

### Comparing `troi-2024.4.26.0/README.md` & `troi-29.0/README.md`

 * *Files identical despite different names*

### Comparing `troi-2024.4.26.0/docs/Makefile` & `troi-29.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `troi-2024.4.26.0/docs/conf.py` & `troi-29.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `troi-2024.4.26.0/docs/dev/index.rst` & `troi-29.0/docs/dev/index.rst`

 * *Files identical despite different names*

### Comparing `troi-2024.4.26.0/docs/elements/index.rst` & `troi-29.0/docs/elements/index.rst`

 * *Files identical despite different names*

### Comparing `troi-2024.4.26.0/docs/elements/listenbrainz.rst` & `troi-29.0/docs/elements/listenbrainz.rst`

 * *Files identical despite different names*

### Comparing `troi-2024.4.26.0/docs/elements/musicbrainz.rst` & `troi-29.0/docs/elements/musicbrainz.rst`

 * *Files identical despite different names*

### Comparing `troi-2024.4.26.0/docs/entities.rst` & `troi-29.0/docs/entities.rst`

 * *Files identical despite different names*

### Comparing `troi-2024.4.26.0/docs/index.rst` & `troi-29.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `troi-2024.4.26.0/docs/installation.rst` & `troi-29.0/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `troi-2024.4.26.0/docs/introduction.rst` & `troi-29.0/docs/introduction.rst`

 * *Files identical despite different names*

### Comparing `troi-2024.4.26.0/docs/lb_radio.rst` & `troi-29.0/docs/lb_radio.rst`

 * *Files identical despite different names*

### Comparing `troi-2024.4.26.0/docs/listenbrainz-logo.svg` & `troi-29.0/docs/listenbrainz-logo.svg`

 * *Files identical despite different names*

### Comparing `troi-2024.4.26.0/docs/make.bat` & `troi-29.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `troi-2024.4.26.0/docs/patches.rst` & `troi-29.0/docs/patches.rst`

 * *Files identical despite different names*

### Comparing `troi-2024.4.26.0/docs/troi-arguments.rst` & `troi-29.0/docs/troi-arguments.rst`

 * *Files identical despite different names*

### Comparing `troi-2024.4.26.0/docs/user-guide.rst` & `troi-29.0/docs/user-guide.rst`

 * *Files identical despite different names*

### Comparing `troi-2024.4.26.0/pyproject.toml` & `troi-29.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `troi-2024.4.26.0/tests/listenbrainz/test_recs.py` & `troi-29.0/tests/listenbrainz/test_recs.py`

 * *Files identical despite different names*

### Comparing `troi-2024.4.26.0/tests/listenbrainz/test_stats.py` & `troi-29.0/tests/listenbrainz/test_stats.py`

 * *Files identical despite different names*

### Comparing `troi-2024.4.26.0/tests/musicbrainz/test_mbid_mapping.py` & `troi-29.0/tests/musicbrainz/test_mbid_mapping.py`

 * *Files identical despite different names*

### Comparing `troi-2024.4.26.0/tests/musicbrainz/test_recording_lookup.py` & `troi-29.0/tests/musicbrainz/test_recording_lookup.py`

 * *Files identical despite different names*

### Comparing `troi-2024.4.26.0/tests/musicbrainz/test_related_artist_credits.py` & `troi-29.0/tests/musicbrainz/test_related_artist_credits.py`

 * *Files identical despite different names*

### Comparing `troi-2024.4.26.0/tests/test_entities.py` & `troi-29.0/tests/test_entities.py`

 * *Files identical despite different names*

### Comparing `troi-2024.4.26.0/tests/test_filters.py` & `troi-29.0/tests/test_filters.py`

 * *Files identical despite different names*

### Comparing `troi-2024.4.26.0/tests/test_operations.py` & `troi-29.0/tests/test_operations.py`

 * *Files identical despite different names*

### Comparing `troi-2024.4.26.0/tests/test_parser.py` & `troi-29.0/tests/test_parser.py`

 * *Files identical despite different names*

### Comparing `troi-2024.4.26.0/tests/test_playlist.py` & `troi-29.0/tests/test_playlist.py`

 * *Files identical despite different names*

### Comparing `troi-2024.4.26.0/tests/test_plist.py` & `troi-29.0/tests/test_plist.py`

 * *Files identical despite different names*

### Comparing `troi-2024.4.26.0/tests/test_sorts.py` & `troi-29.0/tests/test_sorts.py`

 * *Files identical despite different names*

### Comparing `troi-2024.4.26.0/tests/test_tag_utils.py` & `troi-29.0/tests/test_tag_utils.py`

 * *Files identical despite different names*

### Comparing `troi-2024.4.26.0/tests/tools/test_area_lookup.py` & `troi-29.0/tests/tools/test_area_lookup.py`

 * *Files identical despite different names*

### Comparing `troi-2024.4.26.0/troi/__init__.py` & `troi-29.0/troi/__init__.py`

 * *Files identical despite different names*

### Comparing `troi-2024.4.26.0/troi/cli.py` & `troi-29.0/troi/cli.py`

 * *Files identical despite different names*

### Comparing `troi-2024.4.26.0/troi/content_resolver/artist_search.py` & `troi-29.0/troi/content_resolver/artist_search.py`

 * *Files identical despite different names*

### Comparing `troi-2024.4.26.0/troi/content_resolver/cli.py` & `troi-29.0/troi/content_resolver/cli.py`

 * *Files identical despite different names*

### Comparing `troi-2024.4.26.0/troi/content_resolver/content_resolver.py` & `troi-29.0/troi/content_resolver/content_resolver.py`

 * *Files identical despite different names*

### Comparing `troi-2024.4.26.0/troi/content_resolver/database.py` & `troi-29.0/troi/content_resolver/database.py`

 * *Files identical despite different names*

### Comparing `troi-2024.4.26.0/troi/content_resolver/duplicates.py` & `troi-29.0/troi/content_resolver/duplicates.py`

 * *Files identical despite different names*

### Comparing `troi-2024.4.26.0/troi/content_resolver/formats/flac.py` & `troi-29.0/troi/content_resolver/formats/flac.py`

 * *Files identical despite different names*

### Comparing `troi-2024.4.26.0/troi/content_resolver/formats/m4a.py` & `troi-29.0/troi/content_resolver/formats/m4a.py`

 * *Files identical despite different names*

### Comparing `troi-2024.4.26.0/troi/content_resolver/formats/mp3.py` & `troi-29.0/troi/content_resolver/formats/mp3.py`

 * *Files identical despite different names*

### Comparing `troi-2024.4.26.0/troi/content_resolver/formats/ogg_opus.py` & `troi-29.0/troi/content_resolver/formats/ogg_opus.py`

 * *Files identical despite different names*

### Comparing `troi-2024.4.26.0/troi/content_resolver/formats/ogg_vorbis.py` & `troi-29.0/troi/content_resolver/formats/ogg_vorbis.py`

 * *Files identical despite different names*

### Comparing `troi-2024.4.26.0/troi/content_resolver/formats/tag_utils.py` & `troi-29.0/troi/content_resolver/formats/tag_utils.py`

 * *Files identical despite different names*

### Comparing `troi-2024.4.26.0/troi/content_resolver/formats/wma.py` & `troi-29.0/troi/content_resolver/formats/wma.py`

 * *Files identical despite different names*

### Comparing `troi-2024.4.26.0/troi/content_resolver/fuzzy_index.py` & `troi-29.0/troi/content_resolver/fuzzy_index.py`

 * *Files identical despite different names*

### Comparing `troi-2024.4.26.0/troi/content_resolver/lb_radio.py` & `troi-29.0/troi/content_resolver/lb_radio.py`

 * *Files identical despite different names*

### Comparing `troi-2024.4.26.0/troi/content_resolver/metadata_lookup.py` & `troi-29.0/troi/content_resolver/metadata_lookup.py`

 * *Files identical despite different names*

### Comparing `troi-2024.4.26.0/troi/content_resolver/model/recording.py` & `troi-29.0/troi/content_resolver/model/recording.py`

 * *Files identical despite different names*

### Comparing `troi-2024.4.26.0/troi/content_resolver/model/tag.py` & `troi-29.0/troi/content_resolver/model/tag.py`

 * *Files identical despite different names*

### Comparing `troi-2024.4.26.0/troi/content_resolver/model/unresolved_recording.py` & `troi-29.0/troi/content_resolver/model/unresolved_recording.py`

 * *Files identical despite different names*

### Comparing `troi-2024.4.26.0/troi/content_resolver/playlist.py` & `troi-29.0/troi/content_resolver/playlist.py`

 * *Files identical despite different names*

### Comparing `troi-2024.4.26.0/troi/content_resolver/py_sonic_fix.py` & `troi-29.0/troi/content_resolver/py_sonic_fix.py`

 * *Files identical despite different names*

### Comparing `troi-2024.4.26.0/troi/content_resolver/subsonic.py` & `troi-29.0/troi/content_resolver/subsonic.py`

 * *Files identical despite different names*

### Comparing `troi-2024.4.26.0/troi/content_resolver/tag_search.py` & `troi-29.0/troi/content_resolver/tag_search.py`

 * *Files identical despite different names*

### Comparing `troi-2024.4.26.0/troi/content_resolver/top_tags.py` & `troi-29.0/troi/content_resolver/top_tags.py`

 * *Files identical despite different names*

### Comparing `troi-2024.4.26.0/troi/content_resolver/unresolved_recording.py` & `troi-29.0/troi/content_resolver/unresolved_recording.py`

 * *Files identical despite different names*

### Comparing `troi-2024.4.26.0/troi/content_resolver/utils.py` & `troi-29.0/troi/content_resolver/utils.py`

 * *Files identical despite different names*

### Comparing `troi-2024.4.26.0/troi/core.py` & `troi-29.0/troi/core.py`

 * *Files identical despite different names*

### Comparing `troi-2024.4.26.0/troi/external/gpt.py` & `troi-29.0/troi/external/gpt.py`

 * *Files identical despite different names*

### Comparing `troi-2024.4.26.0/troi/filters.py` & `troi-29.0/troi/filters.py`

 * *Files identical despite different names*

### Comparing `troi-2024.4.26.0/troi/listenbrainz/feedback.py` & `troi-29.0/troi/listenbrainz/feedback.py`

 * *Files identical despite different names*

### Comparing `troi-2024.4.26.0/troi/listenbrainz/listens.py` & `troi-29.0/troi/listenbrainz/listens.py`

 * *Files identical despite different names*

### Comparing `troi-2024.4.26.0/troi/listenbrainz/recs.py` & `troi-29.0/troi/listenbrainz/recs.py`

 * *Files identical despite different names*

### Comparing `troi-2024.4.26.0/troi/listenbrainz/stats.py` & `troi-29.0/troi/listenbrainz/stats.py`

 * *Files identical despite different names*

### Comparing `troi-2024.4.26.0/troi/listenbrainz/unused/dataset_fetcher.py` & `troi-29.0/troi/listenbrainz/unused/dataset_fetcher.py`

 * *Files identical despite different names*

### Comparing `troi-2024.4.26.0/troi/listenbrainz/user.py` & `troi-29.0/troi/listenbrainz/user.py`

 * *Files identical despite different names*

### Comparing `troi-2024.4.26.0/troi/local/periodic_jams_local.py` & `troi-29.0/troi/local/periodic_jams_local.py`

 * *Files identical despite different names*

### Comparing `troi-2024.4.26.0/troi/local/recording_resolver.py` & `troi-29.0/troi/local/recording_resolver.py`

 * *Files identical despite different names*

### Comparing `troi-2024.4.26.0/troi/loops.py` & `troi-29.0/troi/loops.py`

 * *Files identical despite different names*

### Comparing `troi-2024.4.26.0/troi/musicbrainz/mbid_mapping.py` & `troi-29.0/troi/musicbrainz/mbid_mapping.py`

 * *Files identical despite different names*

### Comparing `troi-2024.4.26.0/troi/musicbrainz/mbid_reader.py` & `troi-29.0/troi/musicbrainz/mbid_reader.py`

 * *Files identical despite different names*

### Comparing `troi-2024.4.26.0/troi/musicbrainz/recording.py` & `troi-29.0/troi/musicbrainz/recording.py`

 * *Files identical despite different names*

### Comparing `troi-2024.4.26.0/troi/musicbrainz/recording_lookup.py` & `troi-29.0/troi/musicbrainz/recording_lookup.py`

 * *Files identical despite different names*

### Comparing `troi-2024.4.26.0/troi/musicbrainz/related_artist_credits.py` & `troi-29.0/troi/musicbrainz/related_artist_credits.py`

 * *Files identical despite different names*

### Comparing `troi-2024.4.26.0/troi/operations.py` & `troi-29.0/troi/operations.py`

 * *Files identical despite different names*

### Comparing `troi-2024.4.26.0/troi/parse_prompt.py` & `troi-29.0/troi/parse_prompt.py`

 * *Files identical despite different names*

### Comparing `troi-2024.4.26.0/troi/patch.py` & `troi-29.0/troi/patch.py`

 * *Files identical despite different names*

### Comparing `troi-2024.4.26.0/troi/patches/ai_jams.py` & `troi-29.0/troi/patches/ai_jams.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import troi.external.gpt
 import troi.musicbrainz.mbid_mapping
-import troi.patch
 from troi import Playlist
+from troi.patch import Patch
 from troi.playlist import PlaylistMakerElement
 
 
-class AiJamsPatch(troi.patch.Patch):
+class AiJamsPatch(Patch):
     """ Generate a playlist using AI from the given prompt. """
 
     @staticmethod
     def inputs():
         """
         Generate a playlist using AI
```

### Comparing `troi-2024.4.26.0/troi/patches/lb_radio.py` & `troi-29.0/troi/patches/lb_radio.py`

 * *Files identical despite different names*

### Comparing `troi-2024.4.26.0/troi/patches/lb_radio_classes/artist.py` & `troi-29.0/troi/patches/lb_radio_classes/artist.py`

 * *Files identical despite different names*

### Comparing `troi-2024.4.26.0/troi/patches/lb_radio_classes/blend.py` & `troi-29.0/troi/patches/lb_radio_classes/blend.py`

 * *Files identical despite different names*

### Comparing `troi-2024.4.26.0/troi/patches/lb_radio_classes/collection.py` & `troi-29.0/troi/patches/lb_radio_classes/collection.py`

 * *Files identical despite different names*

### Comparing `troi-2024.4.26.0/troi/patches/lb_radio_classes/country.py` & `troi-29.0/troi/patches/lb_radio_classes/country.py`

 * *Files identical despite different names*

### Comparing `troi-2024.4.26.0/troi/patches/lb_radio_classes/playlist.py` & `troi-29.0/troi/patches/lb_radio_classes/playlist.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 
 import requests
 from urllib.parse import quote
 
 from troi import Recording
 from troi import TARGET_NUMBER_OF_RECORDINGS
 
+
 class LBRadioPlaylistRecordingElement(troi.Element):
     """
         Given an LB playlist, fetch its tracks and randomly include recordiungs from it. mode does not
         apply to this element.
     """
 
     NUM_RECORDINGS_TO_COLLECT = TARGET_NUMBER_OF_RECORDINGS * 2
```

### Comparing `troi-2024.4.26.0/troi/patches/lb_radio_classes/recs.py` & `troi-29.0/troi/patches/lb_radio_classes/recs.py`

 * *Files identical despite different names*

### Comparing `troi-2024.4.26.0/troi/patches/lb_radio_classes/stats.py` & `troi-29.0/troi/patches/lb_radio_classes/stats.py`

 * *Files identical despite different names*

### Comparing `troi-2024.4.26.0/troi/patches/lb_radio_classes/tag.py` & `troi-29.0/troi/patches/lb_radio_classes/tag.py`

 * *Files identical despite different names*

### Comparing `troi-2024.4.26.0/troi/patches/periodic_jams.py` & `troi-29.0/troi/patches/periodic_jams.py`

 * *Files identical despite different names*

### Comparing `troi-2024.4.26.0/troi/patches/periodic_jams_local.py` & `troi-29.0/troi/patches/periodic_jams_local.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 from datetime import datetime, timedelta
 
 import troi.listenbrainz.recs
 import troi.musicbrainz.recording_lookup
 from troi import Playlist
+from troi.patch import Patch
 from troi.playlist import PlaylistMakerElement
 
 from troi.local.recording_resolver import RecordingResolverElement
-from troi.content_resolver.model.database import db
 
 DAYS_OF_RECENT_LISTENS_TO_EXCLUDE = 60  # Exclude tracks listened in last X days from the daily jams playlist
 DAILY_JAMS_MIN_RECORDINGS = 25  # the minimum number of recordings we aspire to have in a daily jam, this is not a hard limit
 BATCH_SIZE_RECS = 1000  # the number of recommendations fetched in 1 go
 MAX_RECS_LIMIT = 1000  # the maximum of recommendations available in LB
 
 
-class PeriodicJamsLocalPatch(troi.patch.Patch):
+class PeriodicJamsLocalPatch(Patch):
     """
     """
 
     def __init__(self, args):
         super().__init__(args)
 
     @staticmethod
```

### Comparing `troi-2024.4.26.0/troi/patches/playlist_from_listenbrainz.py` & `troi-29.0/troi/patches/playlist_from_listenbrainz.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import json
 
 from troi import Playlist
 from troi.patch import Patch
 from troi.playlist import PlaylistFromJSPFElement
-import troi.musicbrainz.recording_lookup
 
 
 class TransferPlaylistPatch(Patch):
 
     @staticmethod
     def inputs():
         """
```

### Comparing `troi-2024.4.26.0/troi/patches/playlist_from_mbids.py` & `troi-29.0/troi/patches/playlist_from_mbids.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 import troi
 from troi import Recording
 from troi.musicbrainz.mbid_reader import MBIDReaderElement
 from troi.musicbrainz.recording_lookup import RecordingLookupElement
+from troi.patch import Patch
 from troi.playlist import PlaylistMakerElement
 
 
-class PlaylistFromMBIDsPatch(troi.patch.Patch):
+class PlaylistFromMBIDsPatch(Patch):
     """
     """
 
     def __init__(self, args):
-        troi.patch.Patch.__init__(self, args)
+        super().__init__(args)
 
     @staticmethod
     def inputs():
         """
         Make a playlist from a file containing one MBID per line.
 
         \b
```

### Comparing `troi-2024.4.26.0/troi/patches/recs_to_playlist.py` & `troi-29.0/troi/patches/recs_to_playlist.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from troi import Element, Recording, Playlist, PipelineError
 import troi.listenbrainz.recs
 import troi.playlist
 import troi.filters
 import troi.sorts
 import troi.musicbrainz.recording_lookup
 import troi.musicbrainz.mbid_mapping
+from troi.patch import Patch
 
 
 class RecsPlaylistMakerElement(Element):
     '''
         This element takes in Recordings and spits out a Playlist, which generating a custom name and desc
         for the playlist from the recording data
     '''
@@ -49,21 +50,21 @@
             return [Playlist(name=self.name,
                     description=self.desc,
                     recordings=inputs[0],
                     patch_slug=self.patch_slug,
                     user_name=self.user_name)]
 
 
-class RecommendationsToPlaylistPatch(troi.patch.Patch):
+class RecommendationsToPlaylistPatch(Patch):
     """
         See below for description
     """
 
     def __init__(self, args):
-        troi.patch.Patch.__init__(self, args)
+        super().__init__(args)
 
     @staticmethod
     def inputs():
         """
         Save the current recommended tracks for a given user and type (top or similar).
 
         \b
```

### Comparing `troi-2024.4.26.0/troi/patches/unused/area_random_recordings.py` & `troi-29.0/troi/patches/unused/area_random_recordings.py`

 * *Files identical despite different names*

### Comparing `troi-2024.4.26.0/troi/playlist.py` & `troi-29.0/troi/playlist.py`

 * *Files identical despite different names*

### Comparing `troi-2024.4.26.0/troi/plist.py` & `troi-29.0/troi/plist.py`

 * *Files identical despite different names*

### Comparing `troi-2024.4.26.0/troi/print_recording.py` & `troi-29.0/troi/print_recording.py`

 * *Files identical despite different names*

### Comparing `troi-2024.4.26.0/troi/recording_search_service.py` & `troi-29.0/troi/recording_search_service.py`

 * *Files identical despite different names*

### Comparing `troi-2024.4.26.0/troi/service.py` & `troi-29.0/troi/service.py`

 * *Files identical despite different names*

### Comparing `troi-2024.4.26.0/troi/sorts.py` & `troi-29.0/troi/sorts.py`

 * *Files identical despite different names*

### Comparing `troi-2024.4.26.0/troi/tools/area_lookup.py` & `troi-29.0/troi/tools/area_lookup.py`

 * *Files identical despite different names*

### Comparing `troi-2024.4.26.0/troi/tools/spotify_lookup.py` & `troi-29.0/troi/tools/spotify_lookup.py`

 * *Files identical despite different names*

### Comparing `troi-2024.4.26.0/troi/utils.py` & `troi-29.0/troi/utils.py`

 * *Files identical despite different names*

### Comparing `troi-2024.4.26.0/troi.egg-info/PKG-INFO` & `troi-29.0/troi.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: troi
-Version: 2024.4.26.0
+Version: 29.0
 Summary: ListenBrainz' empathic music recommendation/playlisting engine
 Author-email: MetaBrainz Foundation <support@metabrainz.org>
 Project-URL: Homepage, https://github.com/metabrainz/troi-recommendation-playground
 Project-URL: Documentation, https://troi.readthedocs.io/en/latest/
 Project-URL: Releases, https://github.com/metabrainz/troi-recommendation-playground/releases
 Project-URL: Issues, https://tickets.metabrainz.org/secure/RapidBoard.jspa?rapidView=14&projectKey=LB#
 Classifier: Programming Language :: Python :: 3
```

### Comparing `troi-2024.4.26.0/troi.egg-info/SOURCES.txt` & `troi-29.0/troi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `troi-2024.4.26.0/troi.egg-info/requires.txt` & `troi-29.0/troi.egg-info/requires.txt`

 * *Files identical despite different names*

