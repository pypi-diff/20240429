# Comparing `tmp/dvtag-0.7.0.tar.gz` & `tmp/dvtag-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dvtag-0.7.0.tar", last modified: Sun Apr 28 12:07:14 2024, max compression
+gzip compressed data, was "dvtag-0.7.1.tar", last modified: Sun Apr 28 15:09:05 2024, max compression
```

## Comparing `dvtag-0.7.0.tar` & `dvtag-0.7.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 12:07:14.428568 dvtag-0.7.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-04-28 12:06:57.000000 dvtag-0.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1924 2024-04-28 12:07:14.428568 dvtag-0.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1297 2024-04-28 12:06:57.000000 dvtag-0.7.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 12:07:14.428568 dvtag-0.7.0/dvtag/
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-28 12:06:57.000000 dvtag-0.7.0/dvtag/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-04-28 12:06:57.000000 dvtag-0.7.0/dvtag/doujinvoice.py
--rw-r--r--   0 runner    (1001) docker     (127)     3599 2024-04-28 12:06:57.000000 dvtag-0.7.0/dvtag/dvtag.py
--rw-r--r--   0 runner    (1001) docker     (127)     2447 2024-04-28 12:06:57.000000 dvtag-0.7.0/dvtag/scrape.py
--rw-r--r--   0 runner    (1001) docker     (127)     4609 2024-04-28 12:06:57.000000 dvtag-0.7.0/dvtag/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 12:07:14.428568 dvtag-0.7.0/dvtag.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1924 2024-04-28 12:07:14.000000 dvtag-0.7.0/dvtag.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      314 2024-04-28 12:07:14.000000 dvtag-0.7.0/dvtag.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-28 12:07:14.000000 dvtag-0.7.0/dvtag.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-28 12:07:14.000000 dvtag-0.7.0/dvtag.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-28 12:07:14.000000 dvtag-0.7.0/dvtag.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-28 12:07:14.000000 dvtag-0.7.0/dvtag.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1321 2024-04-28 12:06:57.000000 dvtag-0.7.0/main.py
--rw-r--r--   0 runner    (1001) docker     (127)      702 2024-04-28 12:07:14.432568 dvtag-0.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-28 12:06:57.000000 dvtag-0.7.0/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)     1665 2024-04-28 12:06:57.000000 dvtag-0.7.0/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 15:09:05.880869 dvtag-0.7.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-04-28 15:08:52.000000 dvtag-0.7.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2622 2024-04-28 15:09:05.880869 dvtag-0.7.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1994 2024-04-28 15:08:52.000000 dvtag-0.7.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 15:09:05.880869 dvtag-0.7.1/dvtag/
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-28 15:08:52.000000 dvtag-0.7.1/dvtag/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-04-28 15:08:52.000000 dvtag-0.7.1/dvtag/doujinvoice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3800 2024-04-28 15:08:52.000000 dvtag-0.7.1/dvtag/dvtag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2538 2024-04-28 15:08:52.000000 dvtag-0.7.1/dvtag/scrape.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4710 2024-04-28 15:08:52.000000 dvtag-0.7.1/dvtag/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 15:09:05.880869 dvtag-0.7.1/dvtag.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2622 2024-04-28 15:09:05.000000 dvtag-0.7.1/dvtag.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-04-28 15:09:05.000000 dvtag-0.7.1/dvtag.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-28 15:09:05.000000 dvtag-0.7.1/dvtag.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-28 15:09:05.000000 dvtag-0.7.1/dvtag.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-28 15:09:05.000000 dvtag-0.7.1/dvtag.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-28 15:09:05.000000 dvtag-0.7.1/dvtag.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1321 2024-04-28 15:08:52.000000 dvtag-0.7.1/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)      702 2024-04-28 15:09:05.880869 dvtag-0.7.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-28 15:08:52.000000 dvtag-0.7.1/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1665 2024-04-28 15:08:52.000000 dvtag-0.7.1/utils.py
```

### Comparing `dvtag-0.7.0/LICENSE` & `dvtag-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dvtag-0.7.0/dvtag/dvtag.py` & `dvtag-0.7.1/dvtag/dvtag.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 from mutagen.flac import FLAC
 from mutagen.id3 import APIC, ID3, TALB, TCON, TDRC, TIT2, TPE1, TPE2, TPOS, TRCK, ID3NoHeaderError
 from natsort import os_sorted
 from PIL.Image import Image
 
 from .doujinvoice import DoujinVoice
-from .scrape import scrape
+from .scrape import scrape, ParsingError
 from .utils import extract_titles, get_audio_paths_list, get_image, get_picture, get_png_byte_arr
 
 __all__ = ["tag"]
 
 
 def tag_mp3s(mp3_paths: List[Path], dv: DoujinVoice, png_bytes_arr: BytesIO, disc_number: Optional[int]):
     tags = ID3()
@@ -76,15 +76,22 @@
 
 
 def tag(basepath: Path, workno: str):
     flac_paths_list, mp3_paths_list = get_audio_paths_list(basepath)
     if not flac_paths_list and not mp3_paths_list:
         return
 
-    dv = scrape(workno)
+    try:
+        dv = scrape(workno)
+    except ParsingError:
+        raise
+    except Exception as e:
+        logging.exception(f"An error occurred during scraping metadata for {workno}: {e}.")
+        return
+
     logging.info(f"[{workno}] Ready to tag...")
     logging.info(f" Circle: {dv.circle}")
     logging.info(f" Album:  {dv.name}")
     logging.info(f" Seiyu:  {','.join(dv.seiyus)}")
     logging.info(f" Genre:  {','.join(dv.genres)}")
     logging.info(f" Date:   {dv.sale_date}")
```

### Comparing `dvtag-0.7.0/dvtag/scrape.py` & `dvtag-0.7.1/dvtag/scrape.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,17 +14,24 @@
     """Exception raised when the parsing metadata from web."""
 
     def __init__(self, message: str, workno: str):
         self.workno = workno
         super().__init__(f"{message} for {workno}")
 
 
+def _get_200(url):
+    rsp = session.get(url)
+    if rsp.status_code != 200:
+        rsp.raise_for_status()
+    return rsp
+
+
 def scrape(workno: str) -> DoujinVoice:
     url = f"https://www.dlsite.com/maniax/work/=/product_id/{workno}.html"
-    html = session.get(url).text  # TODO check response code
+    html = _get_200(url).text
 
     if m := re.search(r'data-product-name="(.+)"\s*data-maker-name="(.+)"', html):
         name = m.group(1)
         circle = m.group(2)
     else:
         raise ParsingError(f"no work name found", workno)
 
@@ -44,15 +51,15 @@
     if m := re.search(r"www\.dlsite\.com/.*?/new/=/year/([0-9]{4})/mon/([0-9]{2})/day/([0-9]{2})/", html):
         sale_date = "{}-{}-{}".format(m.group(1), m.group(2), m.group(3))
     else:
         raise ParsingError(f"no sale date found", workno)
 
     # try extracting more accurate information from chobit
     chobit_api = f"https://chobit.cc/api/v1/dlsite/embed?workno={workno}"
-    res = session.get(chobit_api).text
+    res = _get_200(chobit_api).text
 
     try:
         data = json.loads(res[9:-1])
         if data["count"] and (work := data["works"][0])["file_type"] == "audio":
             image_url = work["thumb"].replace("media.dlsite.com/chobit", "file.chobit.cc", 1)
             # we may get a shorter, yet more accurate article title (with no promotion)
             if work["work_name"] in name:
```

### Comparing `dvtag-0.7.0/dvtag/utils.py` & `dvtag-0.7.1/dvtag/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from typing import List, Optional, Tuple
 
 import requests
 from mutagen.flac import Picture
 from mutagen.id3 import PictureType
 from natsort import os_sort_key
 from PIL import Image
-from requests.adapters import HTTPAdapter
+from requests.adapters import HTTPAdapter, Retry
 
 __all__ = [
     "create_request_session",
     "extract_titles",
     "get_audio_paths_list",
     "get_image",
     "get_picture",
@@ -126,15 +126,16 @@
     Args:
         max_retries (int, optional): Maximum retry times. Defaults to 5.
 
     Returns:
         requests.Session: Request session
     """
     session = requests.Session()
-    adapter = HTTPAdapter(max_retries=max_retries)
+    retries = Retry(total=max_retries, backoff_factor=0.1, status_forcelist=[500, 502, 503, 504])
+    adapter = HTTPAdapter(max_retries=retries)
     session.mount("http://", adapter)
     session.mount("https://", adapter)
     return session
 
 
 _title_pat = re.compile(
     r"^(#|■|◆|【|\(|(?:【?tr(?:ack)?|トラック|音轨|とらっく)[\-_‗\s\.．・,：]*)?([\d]+)([\-_‗\s\.．・,：】\)]+|(?=[「『【]))(.+)",
```

### Comparing `dvtag-0.7.0/main.py` & `dvtag-0.7.1/main.py`

 * *Files identical despite different names*

### Comparing `dvtag-0.7.0/setup.cfg` & `dvtag-0.7.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = dvtag
-version = 0.7.0
+version = 0.7.1
 author = Nobe Kanai
 author_email = nobekanai@gmail.com
 description = A tool for tagging your doujin voice library.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/nobekanai/dvtag
 classifiers =
```

### Comparing `dvtag-0.7.0/utils.py` & `dvtag-0.7.1/utils.py`

 * *Files identical despite different names*

