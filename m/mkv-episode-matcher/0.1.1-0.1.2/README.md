# Comparing `tmp/mkv_episode_matcher-0.1.1.tar.gz` & `tmp/mkv_episode_matcher-0.1.2.tar.gz`

## Comparing `mkv_episode_matcher-0.1.1.tar` & `mkv_episode_matcher-0.1.2.tar`

### file list

```diff
@@ -1,4 +1,15 @@
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 mkv_episode_matcher-0.1.1/.gitignore
--rw-r--r--   0        0        0     3130 2020-02-02 00:00:00.000000 mkv_episode_matcher-0.1.1/README.md
--rw-r--r--   0        0        0     2807 2020-02-02 00:00:00.000000 mkv_episode_matcher-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     4351 2020-02-02 00:00:00.000000 mkv_episode_matcher-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 mkv_episode_matcher-0.1.2/libraries/pgs2srt/.git
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 mkv_episode_matcher-0.1.2/libraries/pgs2srt/.gitignore
+-rw-r--r--   0        0        0     1400 2020-02-02 00:00:00.000000 mkv_episode_matcher-0.1.2/libraries/pgs2srt/README.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mkv_episode_matcher-0.1.2/libraries/pgs2srt/__init__.py
+-rw-r--r--   0        0        0     2820 2020-02-02 00:00:00.000000 mkv_episode_matcher-0.1.2/libraries/pgs2srt/imagemaker.py
+-rw-r--r--   0        0        0     4283 2020-02-02 00:00:00.000000 mkv_episode_matcher-0.1.2/libraries/pgs2srt/pgs2srt.py
+-rw-r--r--   0        0        0     7169 2020-02-02 00:00:00.000000 mkv_episode_matcher-0.1.2/libraries/pgs2srt/pgsreader.py
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 mkv_episode_matcher-0.1.2/libraries/pgs2srt/requirements.txt
+-rw-r--r--   0        0        0    10164 2020-02-02 00:00:00.000000 mkv_episode_matcher-0.1.2/libraries/pgs2srt/Libraries/SubZero/SubZero.py
+-rw-r--r--   0        0        0     9957 2020-02-02 00:00:00.000000 mkv_episode_matcher-0.1.2/libraries/pgs2srt/Libraries/SubZero/post_processing.py
+-rw-r--r--   0        0        0   676829 2020-02-02 00:00:00.000000 mkv_episode_matcher-0.1.2/libraries/pgs2srt/Libraries/SubZero/dictionaries/data.py
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 mkv_episode_matcher-0.1.2/.gitignore
+-rw-r--r--   0        0        0     3130 2020-02-02 00:00:00.000000 mkv_episode_matcher-0.1.2/README.md
+-rw-r--r--   0        0        0     2824 2020-02-02 00:00:00.000000 mkv_episode_matcher-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     4351 2020-02-02 00:00:00.000000 mkv_episode_matcher-0.1.2/PKG-INFO
```

### Comparing `mkv_episode_matcher-0.1.1/README.md` & `mkv_episode_matcher-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `mkv_episode_matcher-0.1.1/pyproject.toml` & `mkv_episode_matcher-0.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [tool.hatch.build.targets.sdist]
 include = [
-  "libraries/pgs2srtkg/**/*.py",
+  "/libraries/pgs2srtkg/**/*.py",
+  "/libraries"
 ]
 [project]
 name = "mkv-episode-matcher"
 dynamic = ["version"]
 description = "The MKV Episode Matcher is a tool for identifying TV series episodes from MKV files and renaming the files accordingly."
 readme = "README.md"
 requires-python = ">=3.8"
```

### Comparing `mkv_episode_matcher-0.1.1/PKG-INFO` & `mkv_episode_matcher-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: mkv-episode-matcher
-Version: 0.1.1
+Version: 0.1.2
 Summary: The MKV Episode Matcher is a tool for identifying TV series episodes from MKV files and renaming the files accordingly.
 Project-URL: Documentation, https://github.com/Jsakkos/mkv-episode-matcher#readme
 Project-URL: Issues, https://github.com/Jsakkos/mkv-episode-matcher/issues
 Project-URL: Source, https://github.com/Jsakkos/mkv-episode-matcher
 Author-email: Jsakkos <jonathansakkos@protonmail.com>
 License-Expression: MIT
 Classifier: Development Status :: 4 - Beta
```

