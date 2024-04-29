# Comparing `tmp/TruMusic-1.2.4.tar.gz` & `tmp/trumusic-1.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TruMusic-1.2.4.tar", last modified: Sat Nov 18 22:07:36 2023, max compression
+gzip compressed data, was "trumusic-1.2.5.tar", last modified: Mon Apr 29 15:28:06 2024, max compression
```

## Comparing `TruMusic-1.2.4.tar` & `trumusic-1.2.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-18 22:07:36.265455 TruMusic-1.2.4/
--rw-r--r--   0 runner    (1001) docker     (127)      832 2023-11-18 22:07:36.265455 TruMusic-1.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      285 2023-11-18 22:07:14.000000 TruMusic-1.2.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-18 22:07:36.265455 TruMusic-1.2.4/TruMusic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      832 2023-11-18 22:07:36.000000 TruMusic-1.2.4/TruMusic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      355 2023-11-18 22:07:36.000000 TruMusic-1.2.4/TruMusic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-18 22:07:36.000000 TruMusic-1.2.4/TruMusic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      111 2023-11-18 22:07:36.000000 TruMusic-1.2.4/TruMusic.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       57 2023-11-18 22:07:36.000000 TruMusic-1.2.4/TruMusic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2023-11-18 22:07:36.000000 TruMusic-1.2.4/TruMusic.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      757 2023-11-18 22:07:14.000000 TruMusic-1.2.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-18 22:07:36.265455 TruMusic-1.2.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-18 22:07:36.265455 TruMusic-1.2.4/tru_music/
--rw-r--r--   0 runner    (1001) docker     (127)    15766 2023-11-18 22:07:14.000000 TruMusic-1.2.4/tru_music/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1402 2023-11-18 22:07:14.000000 TruMusic-1.2.4/tru_music/artist_album.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-18 22:07:36.265455 TruMusic-1.2.4/tru_music/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-18 22:07:14.000000 TruMusic-1.2.4/tru_music/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1019 2023-11-18 22:07:14.000000 TruMusic-1.2.4/tru_music/scripts/cleanup.py
--rw-r--r--   0 runner    (1001) docker     (127)     1952 2023-11-18 22:07:14.000000 TruMusic-1.2.4/tru_music/scripts/trumusic.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:28:06.005293 trumusic-1.2.5/
+-rw-r--r--   0 runner    (1001) docker     (127)      832 2024-04-29 15:28:06.001292 trumusic-1.2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-29 15:27:58.000000 trumusic-1.2.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:28:06.001292 trumusic-1.2.5/TruMusic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      832 2024-04-29 15:28:05.000000 trumusic-1.2.5/TruMusic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      355 2024-04-29 15:28:05.000000 trumusic-1.2.5/TruMusic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 15:28:05.000000 trumusic-1.2.5/TruMusic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-29 15:28:05.000000 trumusic-1.2.5/TruMusic.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-29 15:28:05.000000 trumusic-1.2.5/TruMusic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-29 15:28:05.000000 trumusic-1.2.5/TruMusic.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      757 2024-04-29 15:27:58.000000 trumusic-1.2.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 15:28:06.005293 trumusic-1.2.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:28:06.001292 trumusic-1.2.5/tru_music/
+-rw-r--r--   0 runner    (1001) docker     (127)    15766 2024-04-29 15:27:58.000000 trumusic-1.2.5/tru_music/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1441 2024-04-29 15:27:58.000000 trumusic-1.2.5/tru_music/artist_album.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:28:06.001292 trumusic-1.2.5/tru_music/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 15:27:58.000000 trumusic-1.2.5/tru_music/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-04-29 15:27:58.000000 trumusic-1.2.5/tru_music/scripts/cleanup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1952 2024-04-29 15:27:58.000000 trumusic-1.2.5/tru_music/scripts/trumusic.py
```

### Comparing `TruMusic-1.2.4/PKG-INFO` & `trumusic-1.2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TruMusic
-Version: 1.2.4
+Version: 1.2.5
 Summary: Audio file auto-tagger
 Author-email: Jacob Truman <jacob.truman@gmail.com>
 Project-URL: homepage, https://github.com/jacobtruman/TruMusic
 Project-URL: documentation, https://github.com/jacobtruman/TruMusic
 Project-URL: repository, https://github.com/jacobtruman/TruMusic
 Requires-Python: <4,>=3.7
 Description-Content-Type: text/markdown
```

### Comparing `TruMusic-1.2.4/TruMusic.egg-info/PKG-INFO` & `trumusic-1.2.5/TruMusic.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TruMusic
-Version: 1.2.4
+Version: 1.2.5
 Summary: Audio file auto-tagger
 Author-email: Jacob Truman <jacob.truman@gmail.com>
 Project-URL: homepage, https://github.com/jacobtruman/TruMusic
 Project-URL: documentation, https://github.com/jacobtruman/TruMusic
 Project-URL: repository, https://github.com/jacobtruman/TruMusic
 Requires-Python: <4,>=3.7
 Description-Content-Type: text/markdown
```

### Comparing `TruMusic-1.2.4/tru_music/__init__.py` & `trumusic-1.2.5/tru_music/__init__.py`

 * *Files identical despite different names*

### Comparing `TruMusic-1.2.4/tru_music/artist_album.py` & `trumusic-1.2.5/tru_music/artist_album.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from ascii_magic import AsciiArt
 
 class ArtistAlbum:
 
     def __init__(self, item, album):
         artists = item.get('artists')
-        # for some reason the artist is in the "year" field for "other_versions"
-        self.artist = artists[0].get('name') if artists else item.get('year')
+        # for some reason the artist is at index 1 for regular versions and index 0 for "other_versions"
+        self.artist = artists[1].get('name') if len(artists) > 1 else artists[0].get('name')
         self.explicit = item.get('isExplicit')
         self.year = album.get('year')
         self.track_count = album.get('trackCount')
         self._cover_url = None
         self.cover_url = album.get("thumbnails")
         self.tracks = album.get("tracks")
         self.title = item.get('title')
```

### Comparing `TruMusic-1.2.4/tru_music/scripts/cleanup.py` & `trumusic-1.2.5/tru_music/scripts/cleanup.py`

 * *Files identical despite different names*

### Comparing `TruMusic-1.2.4/tru_music/scripts/trumusic.py` & `trumusic-1.2.5/tru_music/scripts/trumusic.py`

 * *Files identical despite different names*

