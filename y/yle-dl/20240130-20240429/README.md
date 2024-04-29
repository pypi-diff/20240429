# Comparing `tmp/yle_dl-20240130.tar.gz` & `tmp/yle_dl-20240429.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yle_dl-20240130.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "yle_dl-20240429.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `yle_dl-20240130.tar` & `yle_dl-20240429.tar`

### file list

```diff
@@ -1,45 +1,45 @@
--rw-r--r--   0        0        0    35147 2023-12-14 17:53:56.836450 yle_dl-20240130/COPYING
--rw-r--r--   0        0        0    27401 2024-01-30 18:15:11.855848 yle_dl-20240130/ChangeLog
--rw-r--r--   0        0        0     4545 2023-12-14 17:53:56.844450 yle_dl-20240130/OS-install-instructions.md
--rw-r--r--   0        0        0     5057 2024-01-30 18:17:33.690575 yle_dl-20240130/README.fi.md
--rw-r--r--   0        0        0     6593 2024-01-30 18:17:33.698575 yle_dl-20240130/README.md
--rw-r--r--   0        0        0     3398 2024-01-30 18:17:33.678574 yle_dl-20240130/README.sv.md
--rw-r--r--   0        0        0     1669 2024-01-28 07:30:32.356320 yle_dl-20240130/pyproject.toml
--rw-r--r--   0        0        0      403 2023-12-14 17:53:56.844450 yle_dl-20240130/releasing.md
--rw-r--r--   0        0        0       69 2023-12-14 17:53:56.844450 yle_dl-20240130/setup.py
--rw-r--r--   0        0        0     1348 2023-12-14 17:53:56.844450 yle_dl-20240130/tests/conftest.py
--rw-r--r--   0        0        0     8169 2024-01-27 08:12:03.609699 yle_dl-20240130/tests/integration/test_areena_it.py
--rw-r--r--   0        0        0     4784 2023-12-14 17:53:56.844450 yle_dl-20240130/tests/integration/test_areena_radio_it.py
--rw-r--r--   0        0        0     1821 2023-12-14 17:53:56.844450 yle_dl-20240130/tests/integration/test_arkisto_it.py
--rw-r--r--   0        0        0     3054 2023-12-14 17:53:56.844450 yle_dl-20240130/tests/integration/test_arkivet_it.py
--rw-r--r--   0        0        0     5156 2024-01-27 08:12:03.609699 yle_dl-20240130/tests/integration/test_uutiset_it.py
--rw-r--r--   0        0        0     2772 2023-12-14 17:53:56.844450 yle_dl-20240130/tests/unit/test_backend.py
--rw-r--r--   0        0        0    17079 2023-12-14 17:53:56.844450 yle_dl-20240130/tests/unit/test_downloader.py
--rw-r--r--   0        0        0     8788 2023-12-14 17:53:56.844450 yle_dl-20240130/tests/unit/test_flavor_filters.py
--rw-r--r--   0        0        0     1475 2023-12-14 17:53:56.844450 yle_dl-20240130/tests/unit/test_timestamp.py
--rw-r--r--   0        0        0    10556 2023-12-14 17:53:56.844450 yle_dl-20240130/tests/unit/test_title_formatter.py
--rw-r--r--   0        0        0     2886 2023-12-14 17:53:56.844450 yle_dl-20240130/tests/utils.py
--rw-r--r--   0        0        0      435 2023-12-14 17:53:56.844450 yle_dl-20240130/yledl.conf.sample
--rw-r--r--   0        0        0     1222 2023-12-14 17:53:56.844450 yle_dl-20240130/yledl/__init__.py
--rw-r--r--   0        0        0      782 2023-12-14 17:53:56.844450 yle_dl-20240130/yledl/__main__.py
--rw-r--r--   0        0        0    20678 2023-12-14 17:53:56.844450 yle_dl-20240130/yledl/backends.py
--rw-r--r--   0        0        0    17758 2023-12-14 17:53:56.844450 yle_dl-20240130/yledl/downloader.py
--rw-r--r--   0        0        0     1161 2023-12-14 17:53:56.844450 yle_dl-20240130/yledl/errors.py
--rw-r--r--   0        0        0      744 2023-12-14 17:53:56.844450 yle_dl-20240130/yledl/exitcodes.py
--rw-r--r--   0        0        0    41045 2024-01-24 19:17:58.630411 yle_dl-20240130/yledl/extractors.py
--rw-r--r--   0        0        0     4366 2023-12-14 17:53:56.844450 yle_dl-20240130/yledl/ffprobe.py
--rw-r--r--   0        0        0     1684 2023-12-14 17:53:56.844450 yle_dl-20240130/yledl/geolocation.py
--rw-r--r--   0        0        0     5417 2023-12-14 17:53:56.844450 yle_dl-20240130/yledl/http.py
--rw-r--r--   0        0        0     7140 2024-01-06 09:18:04.239373 yle_dl-20240130/yledl/io.py
--rw-r--r--   0        0        0     9246 2023-12-14 17:53:56.844450 yle_dl-20240130/yledl/kaltura.py
--rw-r--r--   0        0        0     2070 2023-12-14 17:53:56.844450 yle_dl-20240130/yledl/localization.py
--rw-r--r--   0        0        0     1205 2023-12-14 17:53:56.844450 yle_dl-20240130/yledl/streamfilters.py
--rw-r--r--   0        0        0     1185 2023-12-14 17:53:56.844450 yle_dl-20240130/yledl/streamflavor.py
--rw-r--r--   0        0        0     2736 2023-12-14 17:53:56.844450 yle_dl-20240130/yledl/streamprobe.py
--rw-r--r--   0        0        0      818 2023-12-14 17:53:56.844450 yle_dl-20240130/yledl/subtitles.py
--rw-r--r--   0        0        0     2055 2023-12-14 17:53:56.844450 yle_dl-20240130/yledl/timestamp.py
--rw-r--r--   0        0        0     6780 2023-12-14 17:53:56.844450 yle_dl-20240130/yledl/titleformatter.py
--rw-r--r--   0        0        0     1704 2023-12-14 17:53:56.844450 yle_dl-20240130/yledl/utils.py
--rw-r--r--   0        0        0      722 2024-01-30 18:17:33.662574 yle_dl-20240130/yledl/version.py
--rw-r--r--   0        0        0    22306 2024-01-30 18:18:58.988201 yle_dl-20240130/yledl/yledl.py
--rw-r--r--   0        0        0     8082 1970-01-01 00:00:00.000000 yle_dl-20240130/PKG-INFO
+-rw-r--r--   0        0        0    35147 2024-01-30 18:54:43.788630 yle_dl-20240429/COPYING
+-rw-r--r--   0        0        0    27667 2024-04-29 17:45:24.451819 yle_dl-20240429/ChangeLog
+-rw-r--r--   0        0        0     4545 2024-03-24 08:39:26.083961 yle_dl-20240429/OS-install-instructions.md
+-rw-r--r--   0        0        0     4909 2024-04-28 16:11:49.648110 yle_dl-20240429/README.fi.md
+-rw-r--r--   0        0        0     6445 2024-04-28 16:07:42.734571 yle_dl-20240429/README.md
+-rw-r--r--   0        0        0     3250 2024-04-28 16:12:23.825616 yle_dl-20240429/README.sv.md
+-rw-r--r--   0        0        0     1669 2024-03-24 08:39:26.083961 yle_dl-20240429/pyproject.toml
+-rw-r--r--   0        0        0      403 2024-03-24 08:39:26.083961 yle_dl-20240429/releasing.md
+-rw-r--r--   0        0        0       69 2024-03-24 08:39:26.083961 yle_dl-20240429/setup.py
+-rw-r--r--   0        0        0     1348 2024-01-30 18:54:43.796630 yle_dl-20240429/tests/conftest.py
+-rw-r--r--   0        0        0     8097 2024-04-28 16:05:51.303546 yle_dl-20240429/tests/integration/test_areena_it.py
+-rw-r--r--   0        0        0     4784 2024-03-24 08:39:26.083961 yle_dl-20240429/tests/integration/test_areena_radio_it.py
+-rw-r--r--   0        0        0     1821 2024-03-24 08:39:26.083961 yle_dl-20240429/tests/integration/test_arkisto_it.py
+-rw-r--r--   0        0        0     3054 2024-03-24 08:39:26.083961 yle_dl-20240429/tests/integration/test_arkivet_it.py
+-rw-r--r--   0        0        0     5156 2024-03-24 08:39:26.083961 yle_dl-20240429/tests/integration/test_uutiset_it.py
+-rw-r--r--   0        0        0     2772 2024-03-24 08:39:26.083961 yle_dl-20240429/tests/unit/test_backend.py
+-rw-r--r--   0        0        0    17079 2024-03-24 08:39:26.083961 yle_dl-20240429/tests/unit/test_downloader.py
+-rw-r--r--   0        0        0     8788 2024-03-24 08:39:26.083961 yle_dl-20240429/tests/unit/test_flavor_filters.py
+-rw-r--r--   0        0        0     1475 2024-03-24 08:39:26.083961 yle_dl-20240429/tests/unit/test_timestamp.py
+-rw-r--r--   0        0        0    10556 2024-03-24 08:39:26.083961 yle_dl-20240429/tests/unit/test_title_formatter.py
+-rw-r--r--   0        0        0     2886 2024-01-30 18:54:43.800630 yle_dl-20240429/tests/utils.py
+-rw-r--r--   0        0        0      435 2024-03-24 08:39:26.083961 yle_dl-20240429/yledl.conf.sample
+-rw-r--r--   0        0        0     1222 2024-03-24 08:39:26.083961 yle_dl-20240429/yledl/__init__.py
+-rw-r--r--   0        0        0      782 2024-01-30 18:54:43.800630 yle_dl-20240429/yledl/__main__.py
+-rw-r--r--   0        0        0    20678 2024-03-24 08:39:26.083961 yle_dl-20240429/yledl/backends.py
+-rw-r--r--   0        0        0    18008 2024-04-28 06:41:50.673208 yle_dl-20240429/yledl/downloader.py
+-rw-r--r--   0        0        0     1161 2024-01-30 18:54:43.800630 yle_dl-20240429/yledl/errors.py
+-rw-r--r--   0        0        0      744 2024-01-30 18:54:43.800630 yle_dl-20240429/yledl/exitcodes.py
+-rw-r--r--   0        0        0    42774 2024-04-28 18:32:48.147086 yle_dl-20240429/yledl/extractors.py
+-rw-r--r--   0        0        0     4366 2024-03-24 08:39:26.083961 yle_dl-20240429/yledl/ffprobe.py
+-rw-r--r--   0        0        0     1600 2024-04-28 06:43:29.643666 yle_dl-20240429/yledl/geolocation.py
+-rw-r--r--   0        0        0     5417 2024-04-28 07:02:09.379750 yle_dl-20240429/yledl/http.py
+-rw-r--r--   0        0        0     7140 2024-03-24 08:39:26.083961 yle_dl-20240429/yledl/io.py
+-rw-r--r--   0        0        0     9246 2024-03-24 08:39:26.083961 yle_dl-20240429/yledl/kaltura.py
+-rw-r--r--   0        0        0     2070 2024-01-30 18:54:43.804631 yle_dl-20240429/yledl/localization.py
+-rw-r--r--   0        0        0     1205 2024-03-24 08:39:26.087961 yle_dl-20240429/yledl/streamfilters.py
+-rw-r--r--   0        0        0     1185 2024-03-24 08:39:26.087961 yle_dl-20240429/yledl/streamflavor.py
+-rw-r--r--   0        0        0     2736 2024-03-24 08:39:26.087961 yle_dl-20240429/yledl/streamprobe.py
+-rw-r--r--   0        0        0      818 2024-03-24 08:39:26.087961 yle_dl-20240429/yledl/subtitles.py
+-rw-r--r--   0        0        0     2055 2024-01-30 18:54:43.808631 yle_dl-20240429/yledl/timestamp.py
+-rw-r--r--   0        0        0     6780 2024-03-24 08:39:26.087961 yle_dl-20240429/yledl/titleformatter.py
+-rw-r--r--   0        0        0     1704 2024-01-30 18:54:43.808631 yle_dl-20240429/yledl/utils.py
+-rw-r--r--   0        0        0      722 2024-04-29 17:29:25.813183 yle_dl-20240429/yledl/version.py
+-rw-r--r--   0        0        0    22306 2024-04-28 07:36:00.855802 yle_dl-20240429/yledl/yledl.py
+-rw-r--r--   0        0        0     7934 1970-01-01 00:00:00.000000 yle_dl-20240429/PKG-INFO
```

### Comparing `yle_dl-20240130/COPYING` & `yle_dl-20240429/COPYING`

 * *Files identical despite different names*

### Comparing `yle_dl-20240130/ChangeLog` & `yle_dl-20240429/ChangeLog`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,18 @@
 yle-dl - download videos from Yle servers
 Copyright 2009-2024 Antti Ajanki
 Distributed under the GPL v3 or later
 
+Version 20240429
+
+- New command for recording live TV, the old URL stopped working: yle-dl tv1
+- Support for a new stream type introduced in Areena
+- Series page downloading was partly broken after changes in Areena
+- Some Elävä arkisto/Arkivet pages were broken
+
 Version 20240130
 
 - Fix live download links for Yle Sámi radio, Puhe and Vega radio channels
 - Extract inline videos embedded on yle.fi news pages
 - Downloading was broken on Python 3.8 since a few releases ago
 
 Version 20231214
```

### Comparing `yle_dl-20240130/OS-install-instructions.md` & `yle_dl-20240429/OS-install-instructions.md`

 * *Files identical despite different names*

### Comparing `yle_dl-20240130/README.fi.md` & `yle_dl-20240429/README.fi.md`

 * *Files 5% similar despite different names*

```diff
@@ -159,25 +159,25 @@
 ```
 yle-dl --postprocess scripts/muxmp4 https://areena.yle.fi/1-1864726
 ```
 
 ### Suorat TV-lähetykset
 
 ```
-yle-dl https://areena.yle.fi/tv/suorat/yle-tv1
+yle-dl tv1
 
-yle-dl https://areena.yle.fi/tv/suorat/yle-tv2
+yle-dl tv2
 
-yle-dl https://areena.yle.fi/tv/suorat/yle-teema-fem
+yle-dl teema
 ```
 
 Tallenna tunti (eli 3600 sekuntia) sitten TV1:llä näytettyä lähetystä:
 
 ```
-yle-dl --startposition -3600 https://areena.yle.fi/tv/suorat/yle-tv1
+yle-dl --startposition -3600 tv1
 ```
 
 ### Elävä arkisto
 
 ```
 yle-dl https://yle.fi/aihe/artikkeli/2010/10/28/studio-julmahuvi-roudasta-rospuuttoon
 ```
```

### Comparing `yle_dl-20240130/README.md` & `yle_dl-20240429/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -169,25 +169,25 @@
 ```
 yle-dl --postprocess scripts/muxmp4 https://areena.yle.fi/1-787136
 ```
 
 ### Areena live TV broadcasts
 
 ```
-yle-dl https://areena.yle.fi/tv/suorat/yle-tv1
+yle-dl tv1
 
-yle-dl https://areena.yle.fi/tv/suorat/yle-tv2
+yle-dl tv2
 
-yle-dl https://areena.yle.fi/tv/suorat/yle-teema-fem
+yle-dl teema
 ```
 
 Record the broadcast shown an hour (3600 seconds) ago:
 
 ```
-yle-dl --startposition -3600 https://areena.yle.fi/tv/suorat/yle-tv1
+yle-dl --startposition -3600 tv1
 ```
 
 ### Elävä Arkisto
 
 ```
 yle-dl https://yle.fi/aihe/artikkeli/2010/10/28/studio-julmahuvi-roudasta-rospuuttoon
 ```
```

### Comparing `yle_dl-20240130/README.sv.md` & `yle_dl-20240429/README.sv.md`

 * *Files 6% similar despite different names*

```diff
@@ -106,25 +106,25 @@
 ```
 yle-dl --postprocess scripts/muxmp4 https://areena.yle.fi/1-787136
 ```
 
 ### Inspelning av direkt TV sändningar
 
 ```
-yle-dl https://areena.yle.fi/tv/suorat/yle-tv1
+yle-dl tv1
 
-yle-dl https://areena.yle.fi/tv/suorat/yle-tv2
+yle-dl tv2
 
-yle-dl https://areena.yle.fi/tv/suorat/yle-teema-fem
+yle-dl teema
 ```
 
 Spela in sändningen som visades för en timme (3600 sekunder) sedan:
 
 ```
-yle-dl --startposition -3600 https://areena.yle.fi/tv/suorat/yle-tv1
+yle-dl --startposition -3600 tv1
 ```
 
 ### Arkivet
 
 ```
 yle-dl https://yle.fi/aihe/artikkeli/2010/10/28/studio-julmahuvi-roudasta-rospuuttoon
 ```
```

### Comparing `yle_dl-20240130/pyproject.toml` & `yle_dl-20240429/pyproject.toml`

 * *Files identical despite different names*

### Comparing `yle_dl-20240130/tests/conftest.py` & `yle_dl-20240429/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `yle_dl-20240130/tests/integration/test_areena_it.py` & `yle_dl-20240429/tests/integration/test_areena_it.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,23 +71,23 @@
 
     assert len(urls) == 10
     assert all(['.m3u8' in url for url in urls])
 
 
 @pytest.mark.geoblocked
 def test_areena_live_url():
-    streamurl = fetch_stream_url('https://areena.yle.fi/tv/suorat/yle-tv1')
+    streamurl = fetch_stream_url('tv1')
 
     assert len(streamurl) == 1
     assert '.m3u8' in streamurl[0]
 
 
 @pytest.mark.geoblocked
 def test_areena_live_metadata():
-    metadata = fetch_metadata('https://areena.yle.fi/tv/suorat/yle-tv1')
+    metadata = fetch_metadata('tv1')
 
     assert len(metadata) == 1
     assert len(metadata[0]['flavors']) >= 1
     assert all(f.get('media_type') == 'video' for f in metadata[0]['flavors'])
     assert metadata[0]['region'] == 'Finland'
```

### Comparing `yle_dl-20240130/tests/integration/test_areena_radio_it.py` & `yle_dl-20240429/tests/integration/test_areena_radio_it.py`

 * *Files identical despite different names*

### Comparing `yle_dl-20240130/tests/integration/test_arkisto_it.py` & `yle_dl-20240429/tests/integration/test_arkisto_it.py`

 * *Files identical despite different names*

### Comparing `yle_dl-20240130/tests/integration/test_arkivet_it.py` & `yle_dl-20240429/tests/integration/test_arkivet_it.py`

 * *Files identical despite different names*

### Comparing `yle_dl-20240130/tests/integration/test_uutiset_it.py` & `yle_dl-20240429/tests/integration/test_uutiset_it.py`

 * *Files identical despite different names*

### Comparing `yle_dl-20240130/tests/unit/test_backend.py` & `yle_dl-20240429/tests/unit/test_backend.py`

 * *Files identical despite different names*

### Comparing `yle_dl-20240130/tests/unit/test_downloader.py` & `yle_dl-20240429/tests/unit/test_downloader.py`

 * *Files identical despite different names*

### Comparing `yle_dl-20240130/tests/unit/test_flavor_filters.py` & `yle_dl-20240429/tests/unit/test_flavor_filters.py`

 * *Files identical despite different names*

### Comparing `yle_dl-20240130/tests/unit/test_timestamp.py` & `yle_dl-20240429/tests/unit/test_timestamp.py`

 * *Files identical despite different names*

### Comparing `yle_dl-20240130/tests/unit/test_title_formatter.py` & `yle_dl-20240429/tests/unit/test_title_formatter.py`

 * *Files identical despite different names*

### Comparing `yle_dl-20240130/tests/utils.py` & `yle_dl-20240429/tests/utils.py`

 * *Files identical despite different names*

### Comparing `yle_dl-20240130/yledl/__init__.py` & `yle_dl-20240429/yledl/__init__.py`

 * *Files identical despite different names*

### Comparing `yle_dl-20240130/yledl/__main__.py` & `yle_dl-20240429/yledl/__main__.py`

 * *Files identical despite different names*

### Comparing `yle_dl-20240130/yledl/backends.py` & `yle_dl-20240429/yledl/backends.py`

 * *Files identical despite different names*

### Comparing `yle_dl-20240130/yledl/downloader.py` & `yle_dl-20240429/yledl/downloader.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # This file is part of yle-dl.
 #
-# Copyright 2010-2023 Antti Ajanki and others
+# Copyright 2010-2024 Antti Ajanki and others
 #
 # Yle-dl is free software: you can redistribute it and/or modify it
 # under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
 # Yle-dl is distributed in the hope that it will be useful, but
@@ -14,21 +14,22 @@
 #
 # You should have received a copy of the GNU General Public License
 # along with yle-dl. If not, see <https://www.gnu.org/licenses/>.
 
 import copy
 import logging
 import os
+import re
 from dataclasses import asdict
 from .errors import TransientDownloadError
 from .utils import sane_filename
 from .backends import Subprocess
 from .errors import ExternalApplicationNotFoundError
 from .exitcodes import RD_SUCCESS, RD_FAILED
-from .extractors import extractor_factory, url_language
+from .extractors import extractor_factory
 from .localization import TranslationChooser
 from .io import OutputFileNameGenerator
 from .streamflavor import failed_flavor
 from .ffprobe import NullProbe
 
 
 logger = logging.getLogger('yledl')
@@ -451,16 +452,26 @@
             backend_preference.get(stream.name, -1)
             for stream in x.streams
         )
         return (x.height or 0, backend_score, x.bitrate or 0)
 
     return sortkey
 
+
 def sortkey_max_resolution_min_bitrate(backend_preference):
     def sortkey(x):
         backend_score = max(
             backend_preference.get(stream.name, -1)
             for stream in x.streams
         )
         return (x.height or 0, backend_score, -(x.bitrate or 0))
 
     return sortkey
+
+
+def url_language(url):
+    arenan = re.match(r'^https?://arenan\.yle\.fi/', url) is not None
+    arkivet = re.match(r'^https?://svenska\.yle\.fi/artikel/', url) is not None
+    if arenan or arkivet:
+        return 'swe'
+    else:
+        return 'fin'
```

### Comparing `yle_dl-20240130/yledl/errors.py` & `yle_dl-20240429/yledl/errors.py`

 * *Files identical despite different names*

### Comparing `yle_dl-20240130/yledl/exitcodes.py` & `yle_dl-20240429/yledl/exitcodes.py`

 * *Files identical despite different names*

### Comparing `yle_dl-20240130/yledl/extractors.py` & `yle_dl-20240429/yledl/extractors.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 import json
 import logging
 import os.path
 import re
 from dataclasses import dataclass, field
 from datetime import datetime
 from requests import HTTPError
-from typing import List, Optional
+from typing import Dict, List, Optional
 from urllib.parse import urlparse, parse_qs
 from .backends import HLSAudioBackend, DASHHLSBackend, WgetBackend
 from .http import update_url_query
 from .io import OutputFileNameGenerator
 from .kaltura import YleKalturaApiClient
 from .localization import TranslationChooser
 from .streamflavor import StreamFlavor, failed_flavor
@@ -54,28 +54,22 @@
     elif re.match(r'^https?://yle\.fi/(a|uutiset|urheilu|saa)/', url):
         logger.debug(f'{url} is a news URL')
         return YleUutisetExtractor(language_chooser, httpclient, title_formatter, ffprobe)
     elif (re.match(r'^https?://(areena|arenan)\.yle\.fi/', url) or
           re.match(r'^https?://yle\.fi/', url)):
         logger.debug(f'{url} is an Areena URL')
         return AreenaExtractor(language_chooser, httpclient, title_formatter, ffprobe)
+    elif url.lower() in ['tv1', 'tv2', 'teema']:
+        logger.debug(f'{url} is a live TV channel')
+        return AreenaLiveTVExtractor(language_chooser, httpclient, title_formatter, ffprobe)
     else:
         logger.debug(f'{url} is an unrecognized URL')
         return None
 
 
-def url_language(url):
-    arenan = re.match(r'^https?://arenan\.yle\.fi/', url) is not None
-    arkivet = re.match(r'^https?://svenska\.yle\.fi/artikel/', url) is not None
-    if arenan or arkivet:
-        return 'swe'
-    else:
-        return 'fin'
-
-
 ## Flavors
 
 
 class Flavors:
     @staticmethod
     def media_type(media):
         mtype = media.get('type')
@@ -205,16 +199,20 @@
     expiration_timestamp: Optional[datetime]
     pending: bool
     expired: bool
 
 
 @dataclass(frozen=True)
 class PlaylistData:
+    # The base URL from which to download a playlist
     base_url: str
-    season_parameters: dict
+    # List of query parameters. Each item is a dictionary of query
+    # parameters for one season. If empty, a playlist is downloaded
+    # from the plain base_url.
+    season_parameters: List[Dict]
 
     def season_playlist_urls(self):
         if self.season_parameters:
             for season_query in self.season_parameters:
                 yield update_url_query(self.base_url, season_query)
         else:
             yield self.base_url
@@ -313,19 +311,33 @@
             return False
 
     def _parse_series_playlist(self, html_tree):
         next_data_tag = html_tree.xpath('//script[@id="__NEXT_DATA__"]')
         if next_data_tag:
             next_data = json.loads(next_data_tag[0].text)
             tabs = next_data.get('props', {}).get('pageProps', {}).get('view', {}).get('tabs', [])
-            episodes_tab = [tab for tab in tabs if tab.get('title') in ['Jaksot', 'Avsnitt']]
-            if episodes_tab:
-                episodes_content = episodes_tab[0].get('content', [])
-                if episodes_content:
-                    playlist_data = episodes_content[0]
+            return self._parse_episodes_tab(tabs, True) or self._parse_episodes_tab(tabs, False)
+
+        return None
+
+    def _parse_episodes_tab(self, next_data_tabs, titled_tab):
+        if titled_tab:
+            episodes_tab = [
+                tab for tab in next_data_tabs if tab.get('title') in ['Jaksot', 'Avsnitt']
+            ]
+        else:
+            episodes_tab = [
+                tab for tab in next_data_tabs if tab.get('type') == 'tab' and 'title' not in tab
+            ]
+
+        if episodes_tab:
+            episodes_content = episodes_tab[0].get('content', [])
+            if episodes_content:
+                playlist_data = episodes_content[0]
+                if playlist_data.get('title') not in ['Katso myös', 'Kuuntele myös']:
                     uri = playlist_data.get('source', {}).get('uri')
 
                     series_parameters = {}
                     filters = playlist_data.get('filters', [])
                     if filters:
                         options = filters[0].get('options', [])
                         series_parameters = [x['parameters'] for x in options]
@@ -339,30 +351,30 @@
         if package_tag:
             package_data = json.loads(package_tag[0])
             tabs = package_data.get('tabs', [])
             if tabs:
                 content = tabs[0].get('content', [])
                 if content:
                     uri = content[0].get('source', {}).get('uri')
-                    return PlaylistData(uri, {})
+                    return PlaylistData(uri, [])
 
         return None
 
     def _parse_radio_playlist(self, html_tree):
         state_tag = html_tree.xpath('//script[contains(., "window.STORE_STATE_FROM_SERVER")]')
         if state_tag:
             state_str = state_tag[0].text
             data = json.loads(state_str.split('=', 1)[-1].strip())
             tabs = data.get('viewStore', {}).get('viewPageView', {}).get('tabs', [])
             tabs = [t for t in tabs if t.get('title') in ['Jaksot', 'Avsnitt']]
             if tabs:
                 all_content = tabs[0].get('allContent')
                 if all_content:
                     uri = all_content[0].get('source', {}).get('uri')
-                    return PlaylistData(uri, {})
+                    return PlaylistData(uri, [])
 
         return None
 
     def _download_playlist_or_latest(self, playlist_data, latest_only):
         season_urls = list(enumerate(playlist_data.season_playlist_urls(), start=1))
         if latest_only:
             # Optimization: The latest episode belongs to the latest season
@@ -429,15 +441,15 @@
                     f'Getting a playlist page, season = {season_num}, '
                     f'size = {page_size}, offset = {offset}')
 
                 params = {
                     'offset': str(offset),
                     'limit': str(page_size),
                     'app_id': 'areena-web-items',
-                    'app_key': 'v9No1mV0omg2BppmDkmDL6tGKw1pRFZt',
+                    'app_key': 'wlTs5D9OjIdeS9krPzRQR4I1PYVzoazN',
                 }
                 playlist_page_url = update_url_query(season_url, params)
                 page = self._parse_series_episode_data(playlist_page_url, season_num)
 
                 if page is None:
                     logger.warning(
                         f'Playlist failed at offset {offset}. Some episodes may be missing!')
@@ -794,28 +806,34 @@
             error = [failed_flavor('Manifest URL is missing')]
             return flavors or error
         elif self.is_html5_media(media_id):
             logger.debug('Detected an HTML5 media')
             return self.hls_probe_flavors(hls_manifest_url, False, ffprobe)
         elif self.is_media_67(media_id) or self.is_media_78(media_id):
             return []
+        elif hls_manifest_url:
+            # Fall-back options for new media_id types
+            logger.debug('Detected a possible HLS media')
+            return self.hls_probe_flavors(hls_manifest_url, False, ffprobe)
         else:
             return [failed_flavor('Unknown stream flavor')]
 
     def kaltura_mp4_flavors(self, media_id, pageurl):
         entry_id = self.kaltura_entry_id(media_id)
         kapi_client = YleKalturaApiClient(self.httpclient)
         playback_context = kapi_client.playback_context(entry_id, pageurl)
         if playback_context:
             return kapi_client.parse_stream_flavors(playback_context, pageurl)
         else:
             return []
 
     def is_html5_media(self, media_id):
-        return media_id and media_id.startswith('29-')
+        # 29- is the most common media ID
+        # 84-, hosted on yleawsmpondemand-04.akamaized.net, April 2024
+        return media_id and (media_id.startswith('29-') or media_id.startswith('84-'))
 
     def is_full_hd_media(self, media_id):
         return media_id and media_id.startswith('55-')
 
     def is_media_67(self, media_id):
         # A new hosting alternative (June 2021)? Hosted on yleawsmpodamdipv4.akamaized.net
         return media_id and media_id.startswith('67-')
@@ -942,17 +960,21 @@
         logger.debug(f'preview data:\n{json.dumps(preview_json, indent=2)}')
 
         return AreenaPreviewApiParser(preview_json)
 
     def preview_url(self, program_id):
         return (
             f'https://player.api.yle.fi/v1/preview/{program_id}.json?'
-            'language=fin&ssl=true&countryCode=FI&host=areenaylefi'
+            'language=fin'
+            '&ssl=true'
+            '&countryCode=FI'
+            '&host=areenaylefi'
             '&app_id=player_static_prod'
             '&app_key=8930d72170e48303cf5f3867780d549b'
+            '&isPortabilityRegion=true'
         )
 
     def publish_event_is_current(self, event):
         return event.get('temporalStatus') == 'currently'
 
     def ignore_invalid_download_url(self, url):
         # Sometimes download url is missing the file name
@@ -967,14 +989,30 @@
             m = re.match(r'K(\d+), J\d+', title)
             if m:
                 return {'season': int(m.group(1))}
 
         return {}
 
 
+### Areena live TV ###
+
+class AreenaLiveTVExtractor(AreenaExtractor):
+    def get_playlist(self, url, latest_only=False):
+        return [url]
+
+    def program_id_from_url(self, url):
+        known_channels = {
+            'tv1': 'yle-tv1',
+            'tv2': 'yle-tv2',
+            'teema': 'yle-teema-fem',
+        }
+
+        return known_channels.get(url.lower())
+
+
 ### Areena live radio ###
 
 
 class AreenaLiveRadioExtractor(AreenaExtractor):
     def get_playlist(self, url, latest_only=False):
         return [url]
 
@@ -1003,18 +1041,25 @@
 
 ### Elava Arkisto ###
 
 
 class ElavaArkistoExtractor(AreenaExtractor):
     def get_playlist(self, url, latest_only=False):
         ids = self.get_dataids(url)
+
         if latest_only:
             ids = ids[-1:]
 
-        return [f'https://areena.yle.fi/{x}' for x in ids]
+        if ids:
+            return [f'https://areena.yle.fi/{x}' for x in ids]
+        else:
+            # Fallback to Yle news parser because sometimes Elävä
+            # arkisto pages are published using the same article type
+            # as news articles.
+            return parse_playlist_from_yle_article(url, self.httpclient, latest_only)
 
     def get_dataids(self, url):
         tree = self.httpclient.download_html_tree(url)
         if tree is None:
             return []
 
         return self.ordered_union(self._simple_dataids(tree), self._ydd_dataids(tree))
@@ -1040,62 +1085,66 @@
 
 
 ### News clips at the Yle news site ###
 
 
 class YleUutisetExtractor(AreenaExtractor):
     def get_playlist(self, url, latest_only=False):
-        tree = self.httpclient.download_html_tree(url)
-        if tree is None:
-            return []
-
-        state = None
-        state_script_nodes = tree.xpath(
-            '//script[@type="text/javascript" and '
-            '(contains(text(), "window.__INITIAL__STATE__") or '
-            ' contains(text(), "window.__INITIAL_STATE__"))]/text()')
-        if len(state_script_nodes) > 0:
-            state_json = re.sub(r'^window\.__INITIAL__?STATE__\s*=\s*', '', state_script_nodes[0])
-            state = json.loads(state_json)
-
-        if state is None:
-            state_div_nodes = tree.xpath('//div[@id="initialState"]')
-            if len(state_div_nodes) > 0:
-                state = json.loads(state_div_nodes[0].attrib.get('data-state'))
-
-        if state is None:
-            return []
-
-        data_ids = []
-        article = state.get('pageData', {}).get('article', {})
-        if article.get('mainMedia') is not None:
-            medias = article['mainMedia']
-            data_ids = [media['id'] for media in medias
-                        if media.get('type') in ['VideoBlock', 'video'] and 'id' in media]
-        else:
-            headline_video_id = article.get('headline', {}).get('video', {}).get('id')
-            if headline_video_id:
-                data_ids = [headline_video_id]
-
-        content = article.get('content', [])
-        inline_media = [
-            block['id'] for block in content
-            if block.get('type') in ['AudioBlock', 'audio', 'VideoBlock', 'video'] and 'id' in block
-        ]
-        for id in inline_media:
-            if id not in data_ids:
-                data_ids.append(id)
+        return parse_playlist_from_yle_article(url, self.httpclient, latest_only)
 
-        logger.debug(f"Found Areena data IDs: {','.join(data_ids)}")
 
-        playlist = [self.id_to_areena_url(id) for id in data_ids]
-        if latest_only:
-            playlist = playlist[-1:]
-
-        return playlist
-
-    def id_to_areena_url(self, data_id):
+def parse_playlist_from_yle_article(url, httpclient, latest_only):
+    def id_to_areena_url(data_id):
         if '-' in data_id:
             areena_id = data_id
         else:
             areena_id = f'1-{data_id}'
         return f'https://areena.yle.fi/{areena_id}'
+
+    tree = httpclient.download_html_tree(url)
+    if tree is None:
+        return []
+
+    state = None
+    state_script_nodes = tree.xpath(
+        '//script[@type="text/javascript" and '
+        '(contains(text(), "window.__INITIAL__STATE__") or '
+        ' contains(text(), "window.__INITIAL_STATE__"))]/text()')
+    if len(state_script_nodes) > 0:
+        state_json = re.sub(r'^window\.__INITIAL__?STATE__\s*=\s*', '', state_script_nodes[0])
+        state = json.loads(state_json)
+
+    if state is None:
+        state_div_nodes = tree.xpath('//div[@id="initialState"]')
+        if len(state_div_nodes) > 0:
+            state = json.loads(state_div_nodes[0].attrib.get('data-state'))
+
+    if state is None:
+        return []
+
+    data_ids = []
+    article = state.get('pageData', {}).get('article', {})
+    if article.get('mainMedia') is not None:
+        medias = article['mainMedia']
+        data_ids = [media['id'] for media in medias
+                    if media.get('type') in ['VideoBlock', 'video'] and 'id' in media]
+    else:
+        headline_video_id = article.get('headline', {}).get('video', {}).get('id')
+        if headline_video_id:
+            data_ids = [headline_video_id]
+
+    content = article.get('content', [])
+    inline_media = [
+        block['id'] for block in content
+        if block.get('type') in ['AudioBlock', 'audio', 'VideoBlock', 'video'] and 'id' in block
+    ]
+    for id in inline_media:
+        if id not in data_ids:
+            data_ids.append(id)
+
+    logger.debug(f"Found Areena data IDs: {','.join(data_ids)}")
+
+    playlist = [id_to_areena_url(id) for id in data_ids]
+    if latest_only:
+        playlist = playlist[-1:]
+
+    return playlist
```

### Comparing `yle_dl-20240130/yledl/ffprobe.py` & `yle_dl-20240429/yledl/ffprobe.py`

 * *Files identical despite different names*

### Comparing `yle_dl-20240130/yledl/geolocation.py` & `yle_dl-20240429/yledl/geolocation.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # This file is part of yle-dl.
 #
-# Copyright 2010-2022 Antti Ajanki and others
+# Copyright 2010-2024 Antti Ajanki and others
 #
 # Yle-dl is free software: you can redistribute it and/or modify it
 # under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
 # Yle-dl is distributed in the hope that it will be useful, but
@@ -24,27 +24,23 @@
 
 
 class AreenaGeoLocation:
     def __init__(self, httpclient):
         self.httpclient = httpclient
 
     def located_in_finland(self, referrer):
-        endpoint = 'https://locations.api.yle.fi/v1/address/current?'\
-            'app_id=player_static_prod&'\
-            'app_key=8930d72170e48303cf5f3867780d549b'
-        extra_headers = {
-            'Referer': referrer,
-            'TE': 'Trailers',
-        }
+        endpoint = 'https://locations.api.yle.fi/v3/address/current?' \
+            'app_id=areena-web-items&' \
+            'app_key=wlTs5D9OjIdeS9krPzRQR4I1PYVzoazN'
+        extra_headers = { 'Referer': referrer }
         try:
             r = self.httpclient.get(endpoint, extra_headers)
         except requests.RequestException:
             logger.warning('Failed to check geo restrictions.')
-            logger.warning('Continuing as if no restrictions apply. '
-                           'This may fail later.')
+            logger.warning('Assuming that no restrictions apply. This may fail later.')
             return True
 
         response = r.json()
         logger.debug('Geo query response:')
         logger.debug(json.dumps(response))
 
         return response.get('country_code') == 'FI'
```

### Comparing `yle_dl-20240130/yledl/http.py` & `yle_dl-20240429/yledl/http.py`

 * *Files identical despite different names*

### Comparing `yle_dl-20240130/yledl/io.py` & `yle_dl-20240429/yledl/io.py`

 * *Files identical despite different names*

### Comparing `yle_dl-20240130/yledl/kaltura.py` & `yle_dl-20240429/yledl/kaltura.py`

 * *Files identical despite different names*

### Comparing `yle_dl-20240130/yledl/localization.py` & `yle_dl-20240429/yledl/localization.py`

 * *Files identical despite different names*

### Comparing `yle_dl-20240130/yledl/streamfilters.py` & `yle_dl-20240429/yledl/streamfilters.py`

 * *Files identical despite different names*

### Comparing `yle_dl-20240130/yledl/streamflavor.py` & `yle_dl-20240429/yledl/streamflavor.py`

 * *Files identical despite different names*

### Comparing `yle_dl-20240130/yledl/streamprobe.py` & `yle_dl-20240429/yledl/streamprobe.py`

 * *Files identical despite different names*

### Comparing `yle_dl-20240130/yledl/subtitles.py` & `yle_dl-20240429/yledl/subtitles.py`

 * *Files identical despite different names*

### Comparing `yle_dl-20240130/yledl/timestamp.py` & `yle_dl-20240429/yledl/timestamp.py`

 * *Files identical despite different names*

### Comparing `yle_dl-20240130/yledl/titleformatter.py` & `yle_dl-20240429/yledl/titleformatter.py`

 * *Files identical despite different names*

### Comparing `yle_dl-20240130/yledl/utils.py` & `yle_dl-20240429/yledl/utils.py`

 * *Files identical despite different names*

### Comparing `yle_dl-20240130/yledl/version.py` & `yle_dl-20240429/yledl/version.py`

 * *Files 20% similar despite different names*

```diff
@@ -11,8 +11,8 @@
 # WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU
 # General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with yle-dl. If not, see <https://www.gnu.org/licenses/>.
 
-__version__ = '20240130'
+__version__ = '20240429'
```

### Comparing `yle_dl-20240130/yledl/yledl.py` & `yle_dl-20240429/yledl/yledl.py`

 * *Files identical despite different names*

### Comparing `yle_dl-20240130/PKG-INFO` & `yle_dl-20240429/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yle-dl
-Version: 20240130
+Version: 20240429
 Summary: Download videos from Yle servers
 Author-email: Antti Ajanki <antti.ajanki@iki.fi>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: End Users/Desktop
@@ -204,25 +204,25 @@
 ```
 yle-dl --postprocess scripts/muxmp4 https://areena.yle.fi/1-787136
 ```
 
 ### Areena live TV broadcasts
 
 ```
-yle-dl https://areena.yle.fi/tv/suorat/yle-tv1
+yle-dl tv1
 
-yle-dl https://areena.yle.fi/tv/suorat/yle-tv2
+yle-dl tv2
 
-yle-dl https://areena.yle.fi/tv/suorat/yle-teema-fem
+yle-dl teema
 ```
 
 Record the broadcast shown an hour (3600 seconds) ago:
 
 ```
-yle-dl --startposition -3600 https://areena.yle.fi/tv/suorat/yle-tv1
+yle-dl --startposition -3600 tv1
 ```
 
 ### Elävä Arkisto
 
 ```
 yle-dl https://yle.fi/aihe/artikkeli/2010/10/28/studio-julmahuvi-roudasta-rospuuttoon
 ```
```

