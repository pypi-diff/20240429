# Comparing `tmp/ncmlistdownloader-1.0.4.240427.tar.gz` & `tmp/ncmlistdownloader-1.0.5.240429.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ncmlistdownloader-1.0.4.240427.tar", last modified: Sat Apr 27 08:17:55 2024, max compression
+gzip compressed data, was "ncmlistdownloader-1.0.5.240429.tar", last modified: Mon Apr 29 10:26:14 2024, max compression
```

## Comparing `ncmlistdownloader-1.0.4.240427.tar` & `ncmlistdownloader-1.0.5.240429.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxrwx   0        0        0        0 2024-04-27 08:17:55.211867 ncmlistdownloader-1.0.4.240427/
--rw-rw-rw-   0        0        0    35181 2024-04-22 14:49:08.000000 ncmlistdownloader-1.0.4.240427/LICENSE
--rw-rw-rw-   0        0        0     1409 2024-04-27 08:17:55.210868 ncmlistdownloader-1.0.4.240427/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-27 08:17:55.154052 ncmlistdownloader-1.0.4.240427/ncmlistdownloader/
--rw-rw-rw-   0        0        0     1421 2024-04-27 08:14:31.000000 ncmlistdownloader-1.0.4.240427/ncmlistdownloader/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-27 08:17:55.181093 ncmlistdownloader-1.0.4.240427/ncmlistdownloader/cmd/
--rw-rw-rw-   0        0        0     1736 2024-04-25 10:28:31.000000 ncmlistdownloader-1.0.4.240427/ncmlistdownloader/cmd/__init__.py
--rw-rw-rw-   0        0        0      653 2024-04-25 14:23:37.000000 ncmlistdownloader-1.0.4.240427/ncmlistdownloader/cmd/common.py
--rw-rw-rw-   0        0        0     1661 2024-04-25 14:30:46.000000 ncmlistdownloader-1.0.4.240427/ncmlistdownloader/cmd/download.py
--rw-rw-rw-   0        0        0     2501 2024-04-22 14:56:53.000000 ncmlistdownloader-1.0.4.240427/ncmlistdownloader/cmd/find_from_id.py
--rw-rw-rw-   0        0        0     1664 2024-04-25 10:31:47.000000 ncmlistdownloader-1.0.4.240427/ncmlistdownloader/cmd/json_io.py
-drwxrwxrwx   0        0        0        0 2024-04-27 08:17:55.193269 ncmlistdownloader-1.0.4.240427/ncmlistdownloader/common/
--rw-rw-rw-   0        0        0     2866 2024-04-26 07:14:57.000000 ncmlistdownloader-1.0.4.240427/ncmlistdownloader/common/__init__.py
--rw-rw-rw-   0        0        0     2325 2024-04-22 14:49:08.000000 ncmlistdownloader-1.0.4.240427/ncmlistdownloader/common/encode_sec_key.py
--rw-rw-rw-   0        0        0     2300 2024-04-27 08:15:10.000000 ncmlistdownloader-1.0.4.240427/ncmlistdownloader/common/global_args.py
--rw-rw-rw-   0        0        0     1784 2024-04-22 14:49:08.000000 ncmlistdownloader-1.0.4.240427/ncmlistdownloader/common/thread_test.py
-drwxrwxrwx   0        0        0        0 2024-04-27 08:17:55.196941 ncmlistdownloader-1.0.4.240427/ncmlistdownloader/downloader/
--rw-rw-rw-   0        0        0     6526 2024-04-22 14:49:08.000000 ncmlistdownloader-1.0.4.240427/ncmlistdownloader/downloader/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-27 08:17:55.198941 ncmlistdownloader-1.0.4.240427/ncmlistdownloader/editer/
--rw-rw-rw-   0        0        0     4046 2024-04-27 08:14:43.000000 ncmlistdownloader-1.0.4.240427/ncmlistdownloader/editer/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-27 08:17:55.200986 ncmlistdownloader-1.0.4.240427/ncmlistdownloader/playlist/
--rw-rw-rw-   0        0        0     2388 2024-04-26 09:44:03.000000 ncmlistdownloader-1.0.4.240427/ncmlistdownloader/playlist/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-27 08:17:55.204923 ncmlistdownloader-1.0.4.240427/ncmlistdownloader/song/
--rw-rw-rw-   0        0        0     8428 2024-04-26 07:14:17.000000 ncmlistdownloader-1.0.4.240427/ncmlistdownloader/song/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-27 08:17:55.207928 ncmlistdownloader-1.0.4.240427/ncmlistdownloader.egg-info/
--rw-rw-rw-   0        0        0     1409 2024-04-27 08:17:55.000000 ncmlistdownloader-1.0.4.240427/ncmlistdownloader.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      777 2024-04-27 08:17:55.000000 ncmlistdownloader-1.0.4.240427/ncmlistdownloader.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-27 08:17:55.000000 ncmlistdownloader-1.0.4.240427/ncmlistdownloader.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       70 2024-04-27 08:17:55.000000 ncmlistdownloader-1.0.4.240427/ncmlistdownloader.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       37 2024-04-27 08:17:55.000000 ncmlistdownloader-1.0.4.240427/ncmlistdownloader.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2024-04-27 08:17:55.000000 ncmlistdownloader-1.0.4.240427/ncmlistdownloader.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-27 08:17:55.211867 ncmlistdownloader-1.0.4.240427/setup.cfg
--rw-rw-rw-   0        0        0     1827 2024-04-27 08:14:21.000000 ncmlistdownloader-1.0.4.240427/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-29 10:26:14.502622 ncmlistdownloader-1.0.5.240429/
+-rw-rw-rw-   0        0        0    35181 2024-04-22 14:49:08.000000 ncmlistdownloader-1.0.5.240429/LICENSE
+-rw-rw-rw-   0        0        0     1409 2024-04-29 10:26:14.499626 ncmlistdownloader-1.0.5.240429/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-29 10:26:14.449251 ncmlistdownloader-1.0.5.240429/ncmlistdownloader/
+-rw-rw-rw-   0        0        0     1425 2024-04-29 10:18:45.000000 ncmlistdownloader-1.0.5.240429/ncmlistdownloader/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-29 10:26:14.471713 ncmlistdownloader-1.0.5.240429/ncmlistdownloader/cmd/
+-rw-rw-rw-   0        0        0     1789 2024-04-29 10:16:10.000000 ncmlistdownloader-1.0.5.240429/ncmlistdownloader/cmd/__init__.py
+-rw-rw-rw-   0        0        0      651 2024-04-29 10:21:56.000000 ncmlistdownloader-1.0.5.240429/ncmlistdownloader/cmd/common.py
+-rw-rw-rw-   0        0        0     1685 2024-04-29 10:22:02.000000 ncmlistdownloader-1.0.5.240429/ncmlistdownloader/cmd/download.py
+-rw-rw-rw-   0        0        0     2689 2024-04-29 10:22:08.000000 ncmlistdownloader-1.0.5.240429/ncmlistdownloader/cmd/find_from_id.py
+-rw-rw-rw-   0        0        0     1664 2024-04-29 10:23:33.000000 ncmlistdownloader-1.0.5.240429/ncmlistdownloader/cmd/json_io.py
+drwxrwxrwx   0        0        0        0 2024-04-29 10:26:14.484507 ncmlistdownloader-1.0.5.240429/ncmlistdownloader/common/
+-rw-rw-rw-   0        0        0     2862 2024-04-29 10:21:37.000000 ncmlistdownloader-1.0.5.240429/ncmlistdownloader/common/__init__.py
+-rw-rw-rw-   0        0        0     2161 2024-04-29 10:21:11.000000 ncmlistdownloader-1.0.5.240429/ncmlistdownloader/common/encode_sec_key.py
+-rw-rw-rw-   0        0        0     2376 2024-04-29 10:20:55.000000 ncmlistdownloader-1.0.5.240429/ncmlistdownloader/common/global_args.py
+-rw-rw-rw-   0        0        0     1791 2024-04-29 10:20:35.000000 ncmlistdownloader-1.0.5.240429/ncmlistdownloader/common/thread_test.py
+drwxrwxrwx   0        0        0        0 2024-04-29 10:26:14.486106 ncmlistdownloader-1.0.5.240429/ncmlistdownloader/downloader/
+-rw-rw-rw-   0        0        0     6233 2024-04-29 10:20:23.000000 ncmlistdownloader-1.0.5.240429/ncmlistdownloader/downloader/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-29 10:26:14.488117 ncmlistdownloader-1.0.5.240429/ncmlistdownloader/editer/
+-rw-rw-rw-   0        0        0     3965 2024-04-29 10:20:17.000000 ncmlistdownloader-1.0.5.240429/ncmlistdownloader/editer/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-29 10:26:14.490652 ncmlistdownloader-1.0.5.240429/ncmlistdownloader/playlist/
+-rw-rw-rw-   0        0        0     2296 2024-04-29 10:19:56.000000 ncmlistdownloader-1.0.5.240429/ncmlistdownloader/playlist/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-29 10:26:14.495640 ncmlistdownloader-1.0.5.240429/ncmlistdownloader/song/
+-rw-rw-rw-   0        0        0     8342 2024-04-29 10:16:56.000000 ncmlistdownloader-1.0.5.240429/ncmlistdownloader/song/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-29 10:26:14.497632 ncmlistdownloader-1.0.5.240429/ncmlistdownloader.egg-info/
+-rw-rw-rw-   0        0        0     1409 2024-04-29 10:26:14.000000 ncmlistdownloader-1.0.5.240429/ncmlistdownloader.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      777 2024-04-29 10:26:14.000000 ncmlistdownloader-1.0.5.240429/ncmlistdownloader.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-29 10:26:14.000000 ncmlistdownloader-1.0.5.240429/ncmlistdownloader.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       70 2024-04-29 10:26:14.000000 ncmlistdownloader-1.0.5.240429/ncmlistdownloader.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       37 2024-04-29 10:26:14.000000 ncmlistdownloader-1.0.5.240429/ncmlistdownloader.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2024-04-29 10:26:14.000000 ncmlistdownloader-1.0.5.240429/ncmlistdownloader.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-29 10:26:14.502622 ncmlistdownloader-1.0.5.240429/setup.cfg
+-rw-rw-rw-   0        0        0     1923 2024-04-29 10:24:20.000000 ncmlistdownloader-1.0.5.240429/setup.py
```

### Comparing `ncmlistdownloader-1.0.4.240427/LICENSE` & `ncmlistdownloader-1.0.5.240429/LICENSE`

 * *Files identical despite different names*

### Comparing `ncmlistdownloader-1.0.4.240427/PKG-INFO` & `ncmlistdownloader-1.0.5.240429/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ncmlistdownloader
-Version: 1.0.4.240427
+Version: 1.0.5.240429
 Summary: 获取网易云音乐歌单数据，下载音乐，主动添加元信息。
 Home-page: https://gitee.com/Cooooldwind/163ListDownloader_NexT
 Author: CooooldWind_
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Customer Service
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: End Users/Desktop
```

### Comparing `ncmlistdownloader-1.0.4.240427/ncmlistdownloader/__init__.py` & `ncmlistdownloader-1.0.5.240429/ncmlistdownloader/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,46 +1,48 @@
-'''
+"""
 ncmlistdownloader/__init__.py
-Core.Ver.1.0.4.240427
+Core.Ver.1.0.5.240429
 Author: CooooldWind_
-'''
+"""
+
 from pathlib import Path
 import time
 from ncmlistdownloader.playlist import *
 from ncmlistdownloader.common import *
 from ncmlistdownloader.common.global_args import *
 
+
 def main():
     for i in CMD_START_WORDS:
         print(i)
-    print(f'[*]{CORE_VERSION}')
+    print(f"[*]{CORE_VERSION}")
     id = str(input("ID: "))
     p = Playlist(id)
     p.get_info()
     print("Playlist info-reading succeed.")
     d = str(input("Dir: "))
-    if d == '':
-        d = str(Path.home()) + '/Downloads/ncmld_downloads/'
+    if d == "":
+        d = str(Path.home()) + "/Downloads/ncmld_downloads/"
     fnf = str(input("Filename format: "))
-    if fnf == '':
-        fnf = '$title$ - $artist$'
-    if d[-1] != '/' and d[-1] != '\\':
-        d += '/'
-    d = d.replace('\\', '/')
+    if fnf == "":
+        fnf = "$title$ - $artist$"
+    if d[-1] != "/" and d[-1] != "\\":
+        d += "/"
+    d = d.replace("\\", "/")
     auto_mkdir(d)
     for i in p.track:
         i.filename_format = d + fnf
     p.multiprocessing_get_detail()
     while p.mp_succeed == False:
         time.sleep(1)
     for i in p.track:
         music_filename = i.song_download()
         if music_filename == -1:
-            print(i.title + ' cannot download.')
+            print(i.title + " cannot download.")
             continue
         cover_filename = i.cover_download()
         lyric_filename = i.lyric_get()
         i.attribute_write(music_filename)
         i.cover_write(music_filename, cover_filename)
         i.lyric_write(music_filename, lyric_filename)
-        print(i.title + ' succeed.')
-    print('Succeed. Files at:', d)
+        print(i.title + " succeed.")
+    print("Succeed. Files at:", d)
```

### Comparing `ncmlistdownloader-1.0.4.240427/ncmlistdownloader/cmd/__init__.py` & `ncmlistdownloader-1.0.5.240429/ncmlistdownloader/cmd/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,49 +1,57 @@
-'''
+"""
 ncmlistdownloader/cmd/__init__.py
-Core.Ver.1.0.1.240425a1
+Core.Ver.1.0.5.240429
 Author: CooooldWind_
-'''
+"""
+
 from ncmlistdownloader.song import *
 from ncmlistdownloader.playlist import *
 from ncmlistdownloader.common.global_args import *
 from ncmlistdownloader.cmd.common import *
 from ncmlistdownloader.cmd.json_io import *
 from ncmlistdownloader.cmd.find_from_id import *
 
 cookies = None
 
+
 def main():
     global cookies
     for i in CMD_START_WORDS:
-        print(format_output(raw = i, type = "Info"))
-    cookies = {'MUSIC_U': input_func("Please input your cookies (ONLY MUSIC_U) (if you don't have, just press enter) ")}
-    if cookies["MUSIC_U"] == '':
+        print(format_output(raw=i, type="Info"))
+    cookies = {
+        "MUSIC_U": input_func(
+            "Please input your cookies (ONLY MUSIC_U) (if you don't have, just press enter) "
+        )
+    }
+    if cookies["MUSIC_U"] == "":
         cookies = None
     while True:
         FUNC_CHOICE = [
             "Find Playlist/Song by ID/Url",
             "Load from json file",
             "Search",
             "Exit",
         ]
         for i in range(0, len(FUNC_CHOICE)):
-            if not(i == 2 and cookies == None): print(format_output(f"[{i + 1}] -> {FUNC_CHOICE[i]}", type = "Info"))
-            else: print(format_output(f"[X] -> {FUNC_CHOICE[i]}", type = "Info"))
+            if not (i == 2 and cookies == None):
+                print(format_output(f"[{i + 1}] -> {FUNC_CHOICE[i]}", type="Info"))
+            else:
+                print(format_output(f"[X] -> {FUNC_CHOICE[i]}", type="Info"))
         choice = None
-        while True:    
+        while True:
             choice = int(input_func("Press the number of the function "))
             if choice >= 1 and choice <= len(FUNC_CHOICE):
                 break
             else:
-                print(format_output("Value Error!", type = "Error"))
+                print(format_output("Value Error!", type="Error"))
         if choice == 1:
-            find_from_id(cookies = cookies)
+            find_from_id(cookies=cookies)
         if choice == 4:
-            print(format_output(raw = "Byebye~", type = "Info"))
+            print(format_output(raw="Byebye~", type="Info"))
             break
         if choice == 2:
-            json_load(str(input_func(notice = "Input the file's save location")))
+            json_load(str(input_func(notice="Input the file's save location")))
+
 
 if __name__ == "__main__":
     main()
-
```

### Comparing `ncmlistdownloader-1.0.4.240427/ncmlistdownloader/cmd/common.py` & `ncmlistdownloader-1.0.5.240429/ncmlistdownloader/cmd/common.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,26 +1,28 @@
-'''
+"""
 ncmlistdownloader/cmd/common.py
-Core.Ver.1.0.1.240425a1
+Core.Ver.1.0.5.240429
 Author: CooooldWind_
-'''
+"""
 
 import time
 
 GLOBAL_CONFIG_MODEL = {
-    'song_download': True,
-    'cover_download': True,
-    'lyric_download': True,
-    'attribute_write': True,
-    'cover_write': True,
-    'lyric_write': True,
+    "song_download": True,
+    "cover_download": True,
+    "lyric_download": True,
+    "attribute_write": True,
+    "cover_write": True,
+    "lyric_write": True,
 }
 
-def format_output(raw: str, type = 'Info') -> str:
-    time_now_formated = time.strftime('%H:%M:%S', time.localtime())
+
+def format_output(raw: str, type="Info") -> str:
+    time_now_formated = time.strftime("%H:%M:%S", time.localtime())
     return_str = f"[{type}][{time_now_formated}] {raw}"
     if type == "Input":
         return_str += ">> "
     return return_str
 
+
 def input_func(notice: str):
-    return input(format_output(raw = notice, type = "Input"))
+    return input(format_output(raw=notice, type="Input"))
```

### Comparing `ncmlistdownloader-1.0.4.240427/ncmlistdownloader/cmd/download.py` & `ncmlistdownloader-1.0.5.240429/ncmlistdownloader/cmd/download.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,44 +1,49 @@
-'''
+"""
 ncmlistdownloader/cmd/download.py
-Core.Ver.1.0.1.240425a1
+Core.Ver.1.0.5.240429
 Author: CooooldWind_
-'''
+"""
 
 import time
 from ncmlistdownloader.cmd.common import *
 from ncmlistdownloader.song import *
 
-def download(d = None):
-    if d == None or dict(d).get('type') != 'downloading_list_ncmld':
-        print(format_output(raw = "Value Error!", type = "Error"))
+
+def download(d=None):
+    if d == None or dict(d).get("type") != "downloading_list_ncmld":
+        print(format_output(raw="Value Error!", type="Error"))
         return
     d = dict(d)
-    print(format_output(raw = '$title$ -> title, $artist$ -> artist, $album$ -> album, $id$ -> id, $$ -> $', type = 'Info'))
-    ff = input_func(notice = 'Input filename format')
-    div = input_func(notice = 'Input path')
-    if div[-1] != '/' and div[-1] != '\\':
-        div += '/'
+    print(
+        format_output(
+            raw="$title$ -> title, $artist$ -> artist, $album$ -> album, $id$ -> id, $$ -> $",
+            type="Info",
+        )
+    )
+    ff = input_func(notice="Input filename format")
+    div = input_func(notice="Input path")
+    if div[-1] != "/" and div[-1] != "\\":
+        div += "/"
     download_track: list[Song] = []
-    for j in d['track']:
-        i = j['info']
-        tmp = Song(id = i['id'])
+    for j in d["track"]:
+        i = j["info"]
+        tmp = Song(id=i["id"])
         # tmp.album = i['album']
         # tmp.artist = i['artist']
         # tmp.id = i['id']
         # tmp.title = i['title']
         # tmp.url_info.update({'album_pic': i['pic_url']})
         tmp.filename_format = div + ff
-        '''tmp.filename_info.update({
+        """tmp.filename_info.update({
             'song': tmp.get_formated_filename('mp3'),
             'pic': tmp.get_formated_filename('jpg'),
             'lyric': tmp.get_formated_filename('lrc'),
-        })'''
+        })"""
         download_track.append(tmp)
-    for i in range(0, len(d['track'])):
-        dd = d['global_config']
-        download_track[i].multi_run(d = dd)
-        print(format_output(raw = f'{download_track[i].title} Start.', type = 'Info'))
+    for i in range(0, len(d["track"])):
+        dd = d["global_config"]
+        download_track[i].multi_run(d=dd)
+        print(format_output(raw=f"{download_track[i].title} Start.", type="Info"))
         while download_track[i].is_dl == False:
             time.sleep(1)
-        print(format_output(raw = f'{download_track[i].title} Succeed.', type = 'Info'))
-    
+        print(format_output(raw=f"{download_track[i].title} Succeed.", type="Info"))
```

### Comparing `ncmlistdownloader-1.0.4.240427/ncmlistdownloader/cmd/json_io.py` & `ncmlistdownloader-1.0.5.240429/ncmlistdownloader/cmd/json_io.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,49 +1,49 @@
-'''
+"""
 ncmlistdownloader/cmd/json_io.py
-Core.Ver.1.0.1.240425a1
+Core.Ver.1.0.5.240429
 Author: CooooldWind_
-'''
+"""
 
 from ncmlistdownloader.song import *
 from ncmlistdownloader.playlist import *
 from ncmlistdownloader.cmd.common import *
 from ncmlistdownloader.cmd.download import *
 
 def json_save_list(pl: Playlist):
     path = str(input_func(notice = "Input the file's save location"))
     d = {
-        'type': 'downloading_list_ncmld',
-        'global_config': GLOBAL_CONFIG_MODEL,
-        'track': [],
+        "type": "downloading_list_ncmld",
+        "global_config": GLOBAL_CONFIG_MODEL,
+        "track": [],
     }
     t = []
     for i in pl.track:
         t.append({
-            'type': 'song',
-            'info': {
-                'title': i.title,
-                'artist': i.artist,
-                'album': i.album,
-                'id': i.id,
-                'pic_url': i.url_info['album_pic']
+            "type": "song",
+            "info": {
+                "title": i.title,
+                "artist": i.artist,
+                "album": i.album,
+                "id": i.id,
+                "pic_url": i.url_info["album_pic"]
             },
-            'global': True,
-            'downloading_config': GLOBAL_CONFIG_MODEL,
+            "global": True,
+            "downloading_config": GLOBAL_CONFIG_MODEL,
         })
-    d['track'] = t
-    if path[-5:] != '.json':
-        path += 'ncmld_saved.json'
-    with open(path, 'w+', encoding = 'utf-8') as file:
+    d["track"] = t
+    if path[-5:] != ".json":
+        path += "ncmld_saved.json"
+    with open(path, "w+", encoding = "utf-8") as file:
         json.dump(d, file, ensure_ascii = False, sort_keys = True)
     print(format_output("Saved!", type = "Info"))
 
 def json_load(path: str):
-    with open(path, 'r+', encoding = 'utf-8') as file:
+    with open(path, "r+", encoding = "utf-8") as file:
         d = json.load(file)
-    for i in range(len(d['track'])):
-        now = d['track'][i]
-        print(format_output(type = 'Info', raw = f'Song #{i}:'))
-        print(format_output(type = 'Info', raw = f'Title: {now['info']['title']}'))
-        print(format_output(type = 'Info', raw = f'Artists: {now['info']['artist']}'))
-        # print(format_output(type = 'Info', raw = f''))
-    download(d)
+    for i in range(len(d["track"])):
+        now = d["track"][i]
+        print(format_output(type = "Info", raw = f"Song #{i}:"))
+        print(format_output(type = "Info", raw = f"Title: {now["info"]["title"]}"))
+        print(format_output(type = "Info", raw = f"Artists: {now["info"]["artist"]}"))
+        # print(format_output(type = "Info", raw = f""))
+    download(d)
```

### Comparing `ncmlistdownloader-1.0.4.240427/ncmlistdownloader/common/__init__.py` & `ncmlistdownloader-1.0.5.240429/ncmlistdownloader/common/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,100 +1,107 @@
-'''
+"""
 ncmlistdownloader/Common/__init__.py
 存储常用函数。
-Core.Ver.1.0.0.240425a1
+Core.Ver.1.0.5.240429
 Author: CooooldWind_
-'''
+"""
 
 import os
 
-def url_split(url = str()) -> str:
-    '''
+
+def url_split(url=str()) -> str:
+    """
     把id从url里面提取出来
     ----------
     参数:
     1. `url`(必填): 需要转换的url
-    '''
+    """
     id_return = url.split("?id=")[-1].split("&")[0]
     return id_return
 
-def artist_turn_str(info = [],split_word = ', ') -> str:
-    '''
+
+def artist_turn_str(info=[], split_word=", ") -> str:
+    """
     把歌手列表转换为字符串。
     ----------
     参数:
     1. `info`(必填): 歌手列表
     2. `split_word`(默认 `, ` ): 分隔符
-    '''
+    """
     if not info:
-        raise ValueError("\"info\" must be a list. See comment for detail infomation.")
+        raise ValueError('"info" must be a list. See comment for detail infomation.')
     str_return = ""
     for i in info:
         str_return += i
         if i != info[-1]:
             str_return += split_word
     return str_return
 
-def get_type(filename = str()) -> str:
-    '''
+
+def get_type(filename=str()) -> str:
+    """
     获取文件的后缀名。
     ----------
     参数：
     1. `filename`: 文件名
-    '''
-    return filename[filename.rfind(".") + 1:]
+    """
+    return filename[filename.rfind(".") + 1 :]
+
 
-def get_name(filename = str()) -> str:
-    '''
+def get_name(filename=str()) -> str:
+    """
     获取文件的名称。
     ----------
     参数：
     1. `filename`: 文件名
-    '''
-    return filename[:filename.rfind(".")]
+    """
+    return filename[: filename.rfind(".")]
 
-def clean(filename = str()) -> str:
-    '''
+
+def clean(filename=str()) -> str:
+    """
     清空有悖于标准的字符的函数。
     ----------
     参数：
     1. `filename`: 文件名
-    '''
+    """
     filename_return = filename
-    dirty = [":","*","\"","?","|","<",">","/","\\"]
+    dirty = [":", "*", '"', "?", "|", "<", ">", "/", "\\"]
     for i in dirty:
         filename_return = filename_return.replace(i, "_")
     return filename_return
 
-def auto_mkdir(path = str()):
-    '''
+
+def auto_mkdir(path=str()):
+    """
     创建路径
     ----------
     参数：
     1. `path`: 路径
-    '''
-    now_path = os.getcwd().replace("\\","/")
-    path_re = path.replace("\\","/")
+    """
+    now_path = os.getcwd().replace("\\", "/")
+    path_re = path.replace("\\", "/")
     if path.find(":/") >= 0:
         path_list = path_re.split("/")
         finally_path_list = path_list
     else:
         now_path_list = now_path.split("/")
         path_list = path_re.split("/")
         while path_list[0] == "../":
             path_list = path_list[1:]
             now_path_list = now_path_list[:-1]
         finally_path_list = now_path_list + path_list
     finally_path = ""
     for i in finally_path_list:
         finally_path += i + "/"
         if not os.path.exists(finally_path):
-            os.mkdir(path = finally_path)
+            os.mkdir(path=finally_path)
+
 
-def format(filename = '', title = '', artist = '', album = '', id = '') -> str:
+def format(filename="", title="", artist="", album="", id="") -> str:
     filename_formated = filename
-    filename_formated = filename_formated.replace('$title$', title)
-    filename_formated = filename_formated.replace('$artist$', artist)
-    filename_formated = filename_formated.replace('$album$', album)
-    filename_formated = filename_formated.replace('$id$', id)
-    filename_formated = filename_formated.replace('$$', '$')
+    filename_formated = filename_formated.replace("$title$", title)
+    filename_formated = filename_formated.replace("$artist$", artist)
+    filename_formated = filename_formated.replace("$album$", album)
+    filename_formated = filename_formated.replace("$id$", id)
+    filename_formated = filename_formated.replace("$$", "$")
     return filename_formated
```

### Comparing `ncmlistdownloader-1.0.4.240427/ncmlistdownloader/common/encode_sec_key.py` & `ncmlistdownloader-1.0.5.240429/ncmlistdownloader/common/encode_sec_key.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,66 +1,68 @@
-'''
+"""
 网易云WeAPI解码
-Core.Ver.1.0.0.240410a1
+Core.Ver.1.0.5.240429
 Author: CooooldWind_, 半岛的孤城
 References: 
 1. 网易云解参数（获取网易云歌词，获取评论同理）[https://www.bilibili.com/read/cv12754897/]
-'''
+"""
 
 import random
 import json
 from base64 import b64encode
 import requests
 from Crypto.Cipher import AES
 from ncmlistdownloader.common.global_args import USER_AGENTS, FUNC_F, SEC_KEY
 
+
 class NeteaseParams:
-    '''
+    """
     WeAPI解码类
     ----------
     参数：
     1. `encode_data`: 传入的参数
     2. `url`: API的URL
-    '''
+    """
+
     def __init__(self, encode_data, url):
         self.encode_data = encode_data
         self.url = url
         self.func_e = "010001"
         self.func_f = FUNC_F
         self.func_g = "0CoJUm6Qyw8W8jud"
         self.func_i = "vlgPRPyGhwA6F4Sq"
         self.encode_sec_key = SEC_KEY
+
     def __to_hex(self, encode_data):
-        '''16进制解码'''
+        """16进制解码"""
         temp = 16 - len(encode_data) % 16
         return encode_data + chr(temp) * temp
+
     def __encode_params(self, encode_data, encode_key):
-        '''解码的关键函数(1)'''
+        """解码的关键函数(1)"""
         func_iv = "0102030405060708"
         encode_data = self.__to_hex(encode_data)
-        encode_aes = AES.new(key = encode_key.encode("utf-8"),
-                            IV = func_iv.encode("utf-8"),
-                            mode = AES.MODE_CBC)
+        encode_aes = AES.new(
+            key=encode_key.encode("utf-8"),
+            IV=func_iv.encode("utf-8"),
+            mode=AES.MODE_CBC,
+        )
         base64_sec_key = encode_aes.encrypt(encode_data.encode("utf-8"))
         return str(b64encode(base64_sec_key), "utf-8")
+
     def __get_params(self, encode_data):
-        '''解码的关键函数(2)'''
+        """解码的关键函数(2)"""
         return self.__encode_params(
-            self.__encode_params(
-                encode_data, self.func_g
-            ), self.func_i
+            self.__encode_params(encode_data, self.func_g), self.func_i
         )
-    def get_resource(self, cookies = None):
-        '''获取资源'''
+
+    def get_resource(self, cookies=None):
+        """获取资源"""
         get_data = {
-            'params': self.__get_params(json.dumps(self.encode_data)),
-            'encSecKey': self.encode_sec_key
+            "params": self.__get_params(json.dumps(self.encode_data)),
+            "encSecKey": self.encode_sec_key,
         }
-        get_headers = {
-            'User-Agent': random.choice(USER_AGENTS)
-        }
-        response = requests.post(self.url,
-                             data = get_data,
-                             headers = get_headers,
-                             cookies = cookies,
-                             timeout = 10)
+        get_headers = {"User-Agent": random.choice(USER_AGENTS)}
+        response = requests.post(
+            self.url, data=get_data, headers=get_headers, cookies=cookies, timeout=10
+        )
         return response.json()
```

### Comparing `ncmlistdownloader-1.0.4.240427/ncmlistdownloader/common/global_args.py` & `ncmlistdownloader-1.0.5.240429/ncmlistdownloader/common/global_args.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,53 +1,56 @@
-'''
+"""
 list_downloader/global_args.py
-Core.Ver.1.0.3.240426
+Core.Ver.1.0.5.240429
 Author: CooooldWind_, 是青旨啊
-'''
+"""
+
 FUNC_F_PART = [
-  "00e0b509f6259df8642dbc35662901477df22677ec152b5ff68ace615bb7",
-  "b725152b3ab17a876aea8a5aa76d2e417629ec4ee341f56135fccf695280",
-  "104e0312ecbda92557c93870114af6c9d05c4f7f0c3685b7a46bee255932",
-  "575cce10b424d813cfe4875d3e82047b97ddef52741d546b8e289dc6935b",
-  "3ece0462db0a22b8e7"
+    "00e0b509f6259df8642dbc35662901477df22677ec152b5ff68ace615bb7",
+    "b725152b3ab17a876aea8a5aa76d2e417629ec4ee341f56135fccf695280",
+    "104e0312ecbda92557c93870114af6c9d05c4f7f0c3685b7a46bee255932",
+    "575cce10b424d813cfe4875d3e82047b97ddef52741d546b8e289dc6935b",
+    "3ece0462db0a22b8e7",
 ]
 SEC_KEY_PART = [
-  "6ea19f618d09893013feb207e6953ab0d04831ccf86095147970745a825a",
-  "0f3288ad0bfdb802ffd5876394599d179b65785e679b23ae38035d476872",
-  "f5270c26f7e15f0e2de0da92ac7fdd1de6a965642a67707d3b204d48a3a3",
-  "c66fe536c9e2056d2032c884d764cf419e8ce7bd245f56bde140deccbaed",
-  "83995285ee66ccda"
+    "6ea19f618d09893013feb207e6953ab0d04831ccf86095147970745a825a",
+    "0f3288ad0bfdb802ffd5876394599d179b65785e679b23ae38035d476872",
+    "f5270c26f7e15f0e2de0da92ac7fdd1de6a965642a67707d3b204d48a3a3",
+    "c66fe536c9e2056d2032c884d764cf419e8ce7bd245f56bde140deccbaed",
+    "83995285ee66ccda",
 ]
 M = "Mozilla/5.0 ("
 json_file = {
-  "FUNC_F": "".join(FUNC_F_PART),
-  "LYRIC_API": "https://music.163.com/weapi/song/lyric?csrf_token=",
-  "PLAYLIST_API": "https://music.163.com/weapi/v6/playlist/detail?",
-  "SEC_KEY": "".join(SEC_KEY_PART),
-  "SONG_FILE_API": "https://music.163.com/song/media/outer/url?id=",
-  "SONG_FILE_API_2": "https://music.163.com/weapi/song/enhance/player/url/v1?",
-  "SONG_INFO_API": "https://music.163.com/weapi/v3/song/detail",
-  "USER_AGENTS": [
-    M + "X11; U; Linux; en-US) AppleWebKit/527+ (KHTML, like Gecko, Safari/419.3) Arora/0.6",
-    M + "Windows; U; Windows NT 5.1; en-US; rv:1.8.1.2pre) Gecko/20070215 K-Ninja/2.1.1",
-    M + "X11; Linux i686; U;) Gecko/20070322 Kazehakase/0.4.5"
-  ]
+    "FUNC_F": "".join(FUNC_F_PART),
+    "LYRIC_API": "https://music.163.com/weapi/song/lyric?csrf_token=",
+    "PLAYLIST_API": "https://music.163.com/weapi/v6/playlist/detail?",
+    "SEC_KEY": "".join(SEC_KEY_PART),
+    "SONG_FILE_API": "https://music.163.com/song/media/outer/url?id=",
+    "SONG_FILE_API_2": "https://music.163.com/weapi/song/enhance/player/url/v1?",
+    "SONG_INFO_API": "https://music.163.com/weapi/v3/song/detail",
+    "USER_AGENTS": [
+        M
+        + "X11; U; Linux; en-US) AppleWebKit/527+ (KHTML, like Gecko, Safari/419.3) Arora/0.6",
+        M
+        + "Windows; U; Windows NT 5.1; en-US; rv:1.8.1.2pre) Gecko/20070215 K-Ninja/2.1.1",
+        M + "X11; Linux i686; U;) Gecko/20070322 Kazehakase/0.4.5",
+    ],
 }
-USER_AGENTS = json_file['USER_AGENTS']
-FUNC_F = json_file['FUNC_F']
-SEC_KEY = json_file['SEC_KEY']
-PLAYLIST_API = json_file['PLAYLIST_API']
-SONG_INFO_API = json_file['SONG_INFO_API']
-SONG_FILE_API = json_file['SONG_FILE_API']
-SONG_FILE_API_2 = json_file['SONG_FILE_API_2']
+USER_AGENTS = json_file["USER_AGENTS"]
+FUNC_F = json_file["FUNC_F"]
+SEC_KEY = json_file["SEC_KEY"]
+PLAYLIST_API = json_file["PLAYLIST_API"]
+SONG_INFO_API = json_file["SONG_INFO_API"]
+SONG_FILE_API = json_file["SONG_FILE_API"]
+SONG_FILE_API_2 = json_file["SONG_FILE_API_2"]
 SEARCH_API = "https://music.163.com/weapi/cloudsearch/get/web?csrf_token="
-LYRIC_API = json_file['LYRIC_API']
-CMD_VERSION = 'Ver.1.0.4.240427'
-CORE_VERSION_SETUP = '1.0.4.240427'
-CORE_VERSION = 'Core.Ver.' + CORE_VERSION_SETUP
+LYRIC_API = json_file["LYRIC_API"]
+CMD_VERSION = "Ver.1.0.4.240427"
+CORE_VERSION_SETUP = "1.0.5.240429"
+CORE_VERSION = "Core.Ver." + CORE_VERSION_SETUP
 CMD_START_WORDS = [
     f"163ListDownloader CMD Ver - {CMD_VERSION}",
     "Made by CooooldWind_",
     "Here's the Gitee/GitHub Page, click a star if you like it~",
     "Gitee: https://gitee.com/CooooldWind/163ListDownloader_NexT/issues",
     "GitHub: https://github.com/CooooldWind/163ListDownloader_NexT/issues",
-]
+]
```

### Comparing `ncmlistdownloader-1.0.4.240427/ncmlistdownloader/common/thread_test.py` & `ncmlistdownloader-1.0.5.240429/ncmlistdownloader/common/thread_test.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,62 +1,72 @@
-'''
+"""
 ncmlistdownloader/common/thread_test.py
-Core.Ver.1.0.0.240402a2
+Core.Ver.1.0.5.240429
 Author: CooooldWind_
 Copied from: https://python-parallel-programmning-cookbook.readthedocs.io/zh-cn/latest/chapter2/13_Evaluating_the_performance_of_multithread_applications.html
-'''
+"""
+
 from threading import Thread
 
+
 class threads_object(Thread):
     def run(self):
         function_to_run()
 
+
 class nothreads_object(object):
     def run(self):
         function_to_run()
 
+
 def non_threaded(num_iter):
     funcs: list[Thread] = []
     for i in range(int(num_iter)):
         funcs.append(nothreads_object())
     for i in funcs:
         i.run()
 
+
 def threaded(num_threads):
     funcs: list[Thread] = []
     for i in range(int(num_threads)):
         funcs.append(threads_object())
     for i in funcs:
         i.start()
     for i in funcs:
         i.join()
 
+
 def function_to_run():
     pass
 
+
 def show_results(func_name, results):
     print("%-23s %4.6f seconds" % (func_name, results))
 
+
 def best_thread_single():
     from timeit import Timer
+
     repeat = 50
     number = 1
     num_threads = [1, 2, 4, 8, 16, 32, 64]
     for i in num_threads:
         t = Timer("non_threaded(%s)" % i, "from __main__ import non_threaded")
-        result_a = sum(t.repeat(repeat = repeat, number = number)) / repeat
+        result_a = sum(t.repeat(repeat=repeat, number=number)) / repeat
         t = Timer("threaded(%s)" % i, "from __main__ import threaded")
-        result_b = sum(t.repeat(repeat = repeat, number = number)) / repeat
-        if result_a  * 500 < result_b:
+        result_b = sum(t.repeat(repeat=repeat, number=number)) / repeat
+        if result_a * 500 < result_b:
             return i // 2
 
-def best_thread(time = 10):  
+
+def best_thread(time=10):
     k = 0
     for i in range(time):
         j = best_thread_single()
         print(j)
         k += j
     num_threads = [1, 2, 4, 8, 16, 32, 64]
     k /= time
     for i in num_threads:
         if i > k:
-            return i // 2
+            return i // 2
```

### Comparing `ncmlistdownloader-1.0.4.240427/ncmlistdownloader/downloader/__init__.py` & `ncmlistdownloader-1.0.5.240429/ncmlistdownloader/downloader/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,166 +1,178 @@
-'''
+"""
 ncmlistdownloader/Downloader/__init__.py
-Core.Ver.1.0.0.240404b4-2
+Core.Ver.1.0.5.240429
 Author: CooooldWind_
-'''
+"""
 
 import random
 import time
 import threading
 import requests
 from requests.adapters import HTTPAdapter
 from ncmlistdownloader.common import *
 from ncmlistdownloader.common.encode_sec_key import *
 
+
 def calc_divisional_range(total_size, chunk_sum):
-    '''
+    """
     calc_divisional_range
-    '''
+    """
     if chunk_sum == 1:
         return [[0, total_size - 1]]
     step = total_size // chunk_sum
     arr = list(range(0, total_size, step))
     result = []
     for i in range(len(arr) - 1):
         s_pos, e_pos = arr[i], arr[i + 1] - 1
         result.append([s_pos, e_pos])
     result[-1][-1] = total_size - 1
     return result
 
+
 class OriginFile:
-    '''
+    """
     OriginFile
-    '''
-    def __init__(self, url = ""):
-        self.url = requests.head(url = url, allow_redirects = True).url
-        self.headers = dict(requests.head(url = self.url, allow_redirects = True).headers)
-        try: self.total_size = int(self.headers['Content-Length'])
-        except: self.total_size = -1
+    """
+
+    def __init__(self, url=""):
+        self.url = requests.head(url=url, allow_redirects=True).url
+        self.headers = dict(requests.head(url=self.url, allow_redirects=True).headers)
+        try:
+            self.total_size = int(self.headers["Content-Length"])
+        except:
+            self.total_size = -1
         if self.total_size != -1:
-            self.chunks = calc_divisional_range(self.total_size, (self.total_size // 1048576) + 1)
+            self.chunks = calc_divisional_range(
+                self.total_size, (self.total_size // 1048576) + 1
+            )
 
-    def auto_start(self, filename = ''):
-        '''
+    def auto_start(self, filename=""):
+        """
         自动寻找合适的方式下载。
         默认<=1MB使用单线程，其他多线程。
-        '''
-        if filename == '':
-            filename = self.url[self.url.rfind('/') + 1:]
+        """
+        if filename == "":
+            filename = self.url[self.url.rfind("/") + 1 :]
         if self.total_size <= 1048576 * 1:
-            self.single_thread_start(filename = filename)
+            self.single_thread_start(filename=filename)
         else:
-            self.multi_thread_start(thread_sum = 8, filename = filename)
+            self.multi_thread_start(thread_sum=8, filename=filename)
 
-    def single_thread_start(self, stream = True, max_retries = 3, filename = str()):
-        '''
+    def single_thread_start(self, stream=True, max_retries=3, filename=str()):
+        """
         单线程运行参数。
         异步策略。
-        '''
+        """
         arg_dict = {
-                'url': self.url,
-                'chunk': [0,1],
-                'stream': stream,
-                'max_retries': max_retries,
-                'thread_sum': 1,
-                'filename': filename
-            }
+            "url": self.url,
+            "chunk": [0, 1],
+            "stream": stream,
+            "max_retries": max_retries,
+            "thread_sum": 1,
+            "filename": filename,
+        }
         downloader = Downloader(**arg_dict)
         downloader.single_run()
 
-    def multi_thread_start(self, stream = True, max_retries = 3, thread_sum = 4, filename = str()):
-        '''
+    def multi_thread_start(
+        self, stream=True, max_retries=3, thread_sum=4, filename=str()
+    ):
+        """
         多线程运行参数
-        '''
+        """
         downloader_list: list[Downloader] = []
         for i in self.chunks:
             arg_dict = {
-                'url': self.url,
-                'chunk': i,
-                'stream': stream,
-                'max_retries': max_retries,
-                'thread_sum': thread_sum,
-                'filename': filename
+                "url": self.url,
+                "chunk": i,
+                "stream": stream,
+                "max_retries": max_retries,
+                "thread_sum": thread_sum,
+                "filename": filename,
             }
             downloader_list.append(Downloader(**arg_dict))
         k: list[threading.Thread] = []
         for i in downloader_list:
             i.start()
             k.append(i)
         for i in k:
             i.join()
-            
+
 
 class Downloader(threading.Thread):
-    '''
+    """
     每个（部分）文件的下载
-    '''
-    def __init__(self,
-                 url = "",
-                 chunk = None,
-                 stream = True,
-                 max_retries = 3,
-                 thread_sum = 4,
-                 filename = str()):
+    """
+
+    def __init__(
+        self,
+        url="",
+        chunk=None,
+        stream=True,
+        max_retries=3,
+        thread_sum=4,
+        filename=str(),
+    ):
         if not chunk:
-            raise ValueError("\"chunk\" must be a list.")
+            raise ValueError('"chunk" must be a list.')
         threading.Thread.__init__(self)
         self.start_pos = chunk[0]
         self.end_pos = chunk[1]
         self.url = url
         self.stream = stream
         self.session = requests.Session()
-        self.session.mount('http://', HTTPAdapter(max_retries = max_retries))
-        self.session.mount('https://', HTTPAdapter(max_retries = max_retries))
-        self.source = self.session.get(url = self.url,
-                                  stream = self.stream,
-                                  allow_redirects = True,
-                                  timeout = (5,10),
-                                  headers = {
-                                      "Range": f"bytes={self.start_pos}-{self.end_pos}"
-                                  })
+        self.session.mount("http://", HTTPAdapter(max_retries=max_retries))
+        self.session.mount("https://", HTTPAdapter(max_retries=max_retries))
+        self.source = self.session.get(
+            url=self.url,
+            stream=self.stream,
+            allow_redirects=True,
+            timeout=(5, 10),
+            headers={"Range": f"bytes={self.start_pos}-{self.end_pos}"},
+        )
         self.headers = dict(self.source.headers)
-        self.total_size = int(self.headers['Content-Length'])
+        self.total_size = int(self.headers["Content-Length"])
         self.thread_sum = thread_sum
         self.filename = filename
 
     def single_run(self):
-        '''
+        """
         异步策略进行的下载函数
-        '''
-        self.source = self.session.get(url = self.url,
-                                      stream = self.stream,
-                                      allow_redirects = True,
-                                      timeout = (5,10))
+        """
+        self.source = self.session.get(
+            url=self.url, stream=self.stream, allow_redirects=True, timeout=(5, 10)
+        )
         self.headers = dict(self.source.headers)
-        self.total_size = int(self.headers['Content-Length'])
-        with open(self.filename, 'wb+') as file:
+        self.total_size = int(self.headers["Content-Length"])
+        with open(self.filename, "wb+") as file:
             file.seek(self.start_pos)
             rate = 0
-            for data in self.source.iter_content(chunk_size = 1024):
+            for data in self.source.iter_content(chunk_size=1024):
                 file.write(data)
                 rate += len(data)
-                if random.randint(0,1000) % 200 == 0:
+                if random.randint(0, 1000) % 200 == 0:
                     time.sleep(0.01)
 
     def run(self):
-        '''
+        """
         Threading使用的start参数重定向。
-        '''
+        """
         with threading.Semaphore(self.thread_sum):
-            with open(self.filename, 'wb+') as file:
+            with open(self.filename, "wb+") as file:
                 file.seek(self.start_pos)
                 rate = 0
-                for data in self.source.iter_content(chunk_size = 1024):
+                for data in self.source.iter_content(chunk_size=1024):
                     file.write(data)
                     rate += len(data)
-                    if random.randint(0,1000) % 200 == 0:
+                    if random.randint(0, 1000) % 200 == 0:
                         time.sleep(0.01)
 
-'''
+
+"""
 def download(url = "", filename = "", stream = True, max_retries = 3):
     session = requests.Session()
     session.mount('http://', HTTPAdapter(max_retries = max_retries))
     session.mount('https://', HTTPAdapter(max_retries = max_retries))
     with open(filename, 'wb') as file:
         rate = 0
         source = session.get(url = url,
@@ -173,8 +185,8 @@
                 rate += len(data)
                 if random.randint(0,1000) % 200 == 0:
                     time.sleep(0.01)
         else: file.write(source.content)
     
 def response_get(url = "", data = dict()):
     return NeteaseParams(url = url, encode_data = data).get_resource()
-'''
+"""
```

### Comparing `ncmlistdownloader-1.0.4.240427/ncmlistdownloader/editer/__init__.py` & `ncmlistdownloader-1.0.5.240429/ncmlistdownloader/editer/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,118 +1,120 @@
-'''
+"""
 ncmlistdownloader/Editer/__init__.py
-Core.Ver.1.0.4.240427
+Core.Ver.1.0.5.240429
 Author: CooooldWind_
-'''
+"""
+
 from PIL import Image
 from mutagen.flac import FLAC, Picture
 from mutagen.id3 import ID3, APIC, USLT, Encoding
 from mutagen.easyid3 import EasyID3
 from ncmlistdownloader.common import get_type, artist_turn_str
 
-expection_word_front = "Opening files with the suffix \"."
-lyric_expection_word_front = "Opening cover files with the suffix \"."
-cover_expection_word_front = "Opening cover files with the suffix \"."
-expection_word_end = "\" is not supported."
+expection_word_front = 'Opening files with the suffix ".'
+lyric_expection_word_front = 'Opening cover files with the suffix ".'
+cover_expection_word_front = 'Opening cover files with the suffix ".'
+expection_word_end = '" is not supported.'
+
 
-def attribute_write(filename = str(), info = None):
-    '''
+def attribute_write(filename=str(), info=None):
+    """
     属性写入
     ----------
     参数：
     1. `filename`: 文件名, 字符串, 仅mp3/flac格式
     2. `info`: 信息, 里面需要 `'album'` , `'artist'`, `'title'`
-    '''
+    """
     type = get_type(filename)
     if type == "mp3":
         file = EasyID3(filename)
     elif type == "flac":
         file = FLAC(filename)
     else:
         raise Exception(expection_word_front + type + expection_word_end)
     if not info:
-        raise ValueError("\"info\" must be a dict(). See the comment for detail infomatiom.")
-    file['title'] = info['title']
-    file['album'] = info['album']
-    file['artist'] = artist_turn_str(
-        info = info['artist'],
-        split_word = '; ')
+        raise ValueError(
+            '"info" must be a dict(). See the comment for detail infomatiom.'
+        )
+    file["title"] = info["title"]
+    file["album"] = info["album"]
+    file["artist"] = artist_turn_str(info=info["artist"], split_word="; ")
     file.save()
     return 0
 
-def cover_write(filename = str(), cover_filename = str()):
-    '''
+
+def cover_write(filename=str(), cover_filename=str()):
+    """
     专辑封面写入
     ----------
     参数：
     1. `filename`: 文件名, 字符串, 仅mp3/flac格式
     2. `cover_filename`: 封面的文件名, 字符串, 仅jpg格式
-    '''
+    """
     type = get_type(filename)
     if type == "mp3":
         file = ID3(filename)
     elif type == "flac":
         file = FLAC(filename)
     else:
         raise Exception(expection_word_front + type + expection_word_end)
     cover_type = get_type(cover_filename)
     if cover_type != "jpg" and cover_type != "jpeg":
         raise Exception(cover_expection_word_front + cover_type + expection_word_end)
-    with open(cover_filename, 'rb') as cover_file:
+    with open(cover_filename, "rb") as cover_file:
         print(cover_filename)
         print(filename)
         if type == "mp3":
-            file['APIC'] = APIC(
-                encoding = 3,
-                mime = 'image/jpeg',
-                type = 3,
-                desc = u'Cover',
-                data = cover_file.read()
+            file["APIC"] = APIC(
+                encoding=3,
+                mime="image/jpeg",
+                type=3,
+                desc="Cover",
+                data=cover_file.read(),
             )
-            file.save(v2_version = 3, v1 = 2)
+            file.save(v2_version=3, v1=2)
         elif type == "flac":
             file.clear_pictures()
             cover = Picture()
             cover.data = cover_file.read()
             cover.mime = "image/jpeg"
             file.add_picture(cover)
             file.save()
     return 0
 
-def lyric_write(filename = str(), lyric_filename = str()):
-    '''
+
+def lyric_write(filename=str(), lyric_filename=str()):
+    """
     专辑歌词写入
     ----------
     参数：
     1. `filename`: 文件名, 字符串, 仅mp3/flac格式
     2. `lyric_filename`: 歌词的文件名, 字符串, 仅lrc格式
-    '''
+    """
     type = get_type(filename)
     if type == "mp3":
         file = ID3(filename)
     elif type == "flac":
         file = FLAC(filename)
     else:
         raise Exception(expection_word_front + type + expection_word_end)
     lyric_type = get_type(lyric_filename)
     if lyric_type != "lrc":
         raise Exception(lyric_expection_word_front + lyric_type + expection_word_end)
-    with open(lyric_filename, 'rb+') as lyric_file:
+    with open(lyric_filename, "rb+") as lyric_file:
         lyric = lyric_file.read()
         if type == "mp3":
-            file.setall("USLT",[USLT(
-                encoding = Encoding.UTF8,
-                format = 2,
-                type = 1,
-                text = lyric
-            )])
+            file.setall(
+                "USLT", [USLT(encoding=Encoding.UTF8, format=2, type=1, text=lyric)]
+            )
         elif type == "flac":
-            file['lyrics'] = lyric
+            file["lyrics"] = lyric
     file.save()
     return 0
 
-def cover_compress(edge_len = 800, filename = str()):
+
+def cover_compress(edge_len=800, filename=str()):
     cover_file = Image.open(filename)
     cover_file = cover_file.convert("RGB")
     cover_file_type = cover_file.format
     cover_file_out = cover_file.resize((edge_len, edge_len), Image.NEAREST)
-    cover_file_out.save(filename, cover_file_type)
+    cover_file_out.save(filename, cover_file_type)
```

### Comparing `ncmlistdownloader-1.0.4.240427/ncmlistdownloader/playlist/__init__.py` & `ncmlistdownloader-1.0.5.240429/ncmlistdownloader/playlist/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,68 +1,73 @@
-'''
+"""
 ncmlistdownloader/playlist/__init__.py
-Core.Ver.1.0.3.240426
+Core.Ver.1.0.5.240429
 Author: CooooldWind_
-'''
+"""
+
 from ncmlistdownloader.common import *
 from ncmlistdownloader.common.encode_sec_key import *
 from ncmlistdownloader.common.global_args import *
 from ncmlistdownloader.song import *
 import threading
 
-class Playlist():
+
+class Playlist:
     def __init__(self, id: str):
         self.id = id
         if self.id.find("163.com") != -1:
-            self.id = url_split(url = self.id)
+            self.id = url_split(url=self.id)
         self.track: list[Song] = []
         self.creator_id = ""
         self.raw_info = {}
         self.track_count = int(0)
         self.creator = ""
         self.track_id = []
         self.title = ""
         self.mp_succeed = False
 
-    def get_info(self, cookies = None):
-        self.raw_info = NeteaseParams(url = PLAYLIST_API,
-                                      encode_data = {
-                                          'csrf_token': '',
-                                          'id': self.id,
-                                      }).get_resource(cookies = cookies)
-        if self.raw_info['code'] != 200:
+    def get_info(self, cookies=None):
+        self.raw_info = NeteaseParams(
+            url=PLAYLIST_API,
+            encode_data={
+                "csrf_token": "",
+                "id": self.id,
+            },
+        ).get_resource(cookies=cookies)
+        if self.raw_info["code"] != 200:
             return -1
-        self.creator_id = self.raw_info['playlist']['userId']
-        self.track_count = self.raw_info['playlist']['trackCount']
-        self.creator = self.raw_info['playlist']['creator']['nickname']
-        self.title = self.raw_info['playlist']['name']
-        for i in self.raw_info['playlist']['trackIds']:
-            self.track_id.append(str(i['id']))
+        self.creator_id = self.raw_info["playlist"]["userId"]
+        self.track_count = self.raw_info["playlist"]["trackCount"]
+        self.creator = self.raw_info["playlist"]["creator"]["nickname"]
+        self.title = self.raw_info["playlist"]["name"]
+        for i in self.raw_info["playlist"]["trackIds"]:
+            self.track_id.append(str(i["id"]))
         for truck_id in self.track_id:
-            self.track.append(Song(id = truck_id))
+            self.track.append(Song(id=truck_id))
         return self.raw_info
-    
+
     def get_detail_info(self):
         threads: list[threading.Thread] = []
         for i in self.track:
-            thread = threading.Thread(target = i.multi_get_info)
+            thread = threading.Thread(target=i.multi_get_info)
             thread.start()
             threads.append(thread)
         for i in threads:
             i.join()
         self.mp_succeed = True
 
-    def auto_get_info(self, cookies = dict()):
-        if self.get_info(cookies = cookies) != -1:
+    def auto_get_info(self, cookies=dict()):
+        if self.get_info(cookies=cookies) != -1:
             self.get_detail_info()
-        else: return -1
+        else:
+            return -1
 
     def done_sum(self):
         count = 0
         for i in self.track:
             if i.is_get == True:
                 count += 1
         return count
-    
+
     def multiprocessing_get_detail(self):
-        p = threading.Thread(target = self.get_detail_info)
+        p = threading.Thread(target=self.get_detail_info)
         p.start()
```

### Comparing `ncmlistdownloader-1.0.4.240427/ncmlistdownloader/song/__init__.py` & `ncmlistdownloader-1.0.5.240429/ncmlistdownloader/song/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,244 +1,248 @@
-'''
+"""
 ncmlistdownloader/song/__init__.py
-Core.Ver.1.0.0.240426
+Core.Ver.1.0.5.240429
 Author: CooooldWind_
-'''
+"""
 
 from ncmlistdownloader.common import *
 from ncmlistdownloader.common.encode_sec_key import *
 from ncmlistdownloader.common.thread_test import best_thread
 from ncmlistdownloader.downloader import *
 from ncmlistdownloader.common.global_args import *
 from ncmlistdownloader.common.encode_sec_key import *
 from ncmlistdownloader.editer import *
 
-class Song():
-    '''
+
+class Song:
+    """
     Song类
     ----------
     存储歌曲信息，以及各种函数。
-    常用的有如下: 
+    常用的有如下:
     1. `name` / `album` / `artist`
     2. `downloading_state` / `downloading_value`
     3. `raw_info` / `processed_info` / `url_info`
-    参数: 
+    参数:
     1. `id`: 歌曲id (其实传入url也行)
-    '''
+    """
 
     def __init__(self, id: str):
         self.id = id
         if self.id.find("163.com") != -1:
-            self.id = url_split(url = self.id)
+            self.id = url_split(url=self.id)
         self.title = ""
         self.artist = []
         self.artist_str = ""
         self.album = ""
         self.downloading_state = 0
         self.downloading_value = 0.00
         self.encode_data = {
-                'c': str([{'id':str(self.id)}]),
-                'csrf_token': '',
-            }
+            "c": str([{"id": str(self.id)}]),
+            "csrf_token": "",
+        }
         self.lyric_encode_data = {
-            'csrf_token': '',
-            'id': str(str(self.id)),
-            'lv': -1,
-            'tv': -1,
+            "csrf_token": "",
+            "id": str(str(self.id)),
+            "lv": -1,
+            "tv": -1,
         }
         self.raw_info = {}
         self.processed_info = {}
         self.url_info = {}
         self.filename_info = {}
-        self.filename_format = '$title$ - $artist$'
+        self.filename_format = "$title$ - $artist$"
         self.is_get = False
         self.is_dl = False
 
     def __str__(self):
-        '''
+        """
         返回存有歌曲信息的字符串。
         ----------
         无参数。
         如果直接`print`这个类就是调用这个函数了。
-        '''
+        """
         return str(self.processed_info)
-    
+
     def get_formated_filename(self, suffix):
-        formated = format(filename = self.filename_format,
-                          artist = self.artist_str,
-                          album = self.album,
-                          id = self.id,
-                          title = self.title)
-        if formated.rfind('/') != -1:
-            formated = formated[:formated.rfind('/') + 1] + clean(formated[formated.rfind('/') + 1:])
+        formated = format(
+            filename=self.filename_format,
+            artist=self.artist_str,
+            album=self.album,
+            id=self.id,
+            title=self.title,
+        )
+        if formated.rfind("/") != -1:
+            formated = formated[: formated.rfind("/") + 1] + clean(
+                formated[formated.rfind("/") + 1 :]
+            )
         else:
             formated = clean(formated)
-        formated += ('.' + suffix)
+        formated += "." + suffix
         return formated
 
     def get_info(self):
-        '''
+        """
         获取歌曲信息
         ----------
         无参数。
-        '''
+        """
         self.raw_info = NeteaseParams(
-            url = SONG_INFO_API,
-            encode_data = self.encode_data).get_resource()['songs'][0]
-        self.title = self.raw_info['name']
-        self.album = self.raw_info['al']['name']
-        for i in self.raw_info['ar']:
-            self.artist.append(i['name'])
+            url=SONG_INFO_API, encode_data=self.encode_data
+        ).get_resource()["songs"][0]
+        self.title = self.raw_info["name"]
+        self.album = self.raw_info["al"]["name"]
+        for i in self.raw_info["ar"]:
+            self.artist.append(i["name"])
         self.artist_str = artist_turn_str(self.artist)
         self.processed_info = {
-            'album': self.album,
-            'title': self.title,
-            'artist': self.artist,
-            'id': self.id,
-        }
-        self.url_info.update({
-            'album_pic': self.raw_info['al']['picUrl'],
-            'song_file': SONG_FILE_API + self.id,
-        })
+            "album": self.album,
+            "title": self.title,
+            "artist": self.artist,
+            "id": self.id,
+        }
+        self.url_info.update(
+            {
+                "album_pic": self.raw_info["al"]["picUrl"],
+                "song_file": SONG_FILE_API + self.id,
+            }
+        )
         self.filename_info = {
-            'song': self.get_formated_filename('mp3'),
-            'pic': self.get_formated_filename('jpg'),
-            'lyric': self.get_formated_filename('lrc'),
+            "song": self.get_formated_filename("mp3"),
+            "pic": self.get_formated_filename("jpg"),
+            "lyric": self.get_formated_filename("lrc"),
         }
         self.is_get = True
         return self.raw_info
-    
+
     def multi_get_info(self):
-        '''
+        """
         获取歌曲信息（多线程用）
         ----------
         无参数。
-        '''
+        """
         with threading.Semaphore(8):
             self.get_info()
 
-    def song_download_enhanced(self, level: str, cookies = None):
+    def song_download_enhanced(self, level: str, cookies=None):
         flag = True
-        level_key = [
-            'standard',
-            'higher',
-            'exhigh',
-            'lossless'
-        ]
+        level_key = ["standard", "higher", "exhigh", "lossless"]
         for i in level_key:
             if i == level:
                 flag = False
         if flag:
-            raise Exception('Error at inputing \'level\'.')
-        '''
+            raise Exception("Error at inputing 'level'.")
+        """
         data的数据格式：
         {
             “ids”:str([id]),
             “level”:“standard”,
             “encodeType”:“aac”,
             “csrf_token”: “”
         }
         其中id表示歌曲的id号，
         level是音乐品质，
         标准为standard，
         较高音质为higher，
         极高音质exhigh，
         无损音质关键词为lossless。
-        '''
+        """
         enhance_encode_data = {
-            'ids': str([self.id]),
-            'level': level,
-            'encodeType': 'mp3',
-            'csrf_token': '',
+            "ids": str([self.id]),
+            "level": level,
+            "encodeType": "mp3",
+            "csrf_token": "",
         }
-        if level == 'lossless': enhance_encode_data['encodeType'] = 'aac'
+        if level == "lossless":
+            enhance_encode_data["encodeType"] = "aac"
         enhanced_info = NeteaseParams(
-            encode_data = enhance_encode_data,
-            url = SONG_FILE_API_2
-        ).get_resource(cookies = cookies)
+            encode_data=enhance_encode_data, url=SONG_FILE_API_2
+        ).get_resource(cookies=cookies)
         return enhanced_info
 
     def song_download(self):
         # filename = self.get_formated_filename('mp3')
-        filename = self.filename_info['song']
-        file_origin = OriginFile(self.url_info['song_file'])
+        filename = self.filename_info["song"]
+        file_origin = OriginFile(self.url_info["song_file"])
         if file_origin.total_size <= 0:
             return -1
-        file_origin.single_thread_start(filename = filename)
+        file_origin.single_thread_start(filename=filename)
         return filename
 
     def cover_download(self):
-        filename = self.filename_info['pic']
+        filename = self.filename_info["pic"]
         # filename = self.get_formated_filename('jpg')
-        file_origin = OriginFile(self.url_info['album_pic'])
+        file_origin = OriginFile(self.url_info["album_pic"])
         if file_origin.total_size == -1:
             return -1
-        file_origin.auto_start(filename = filename)
+        file_origin.auto_start(filename=filename)
         return filename
 
     def lyric_get(self):
-        self.lyric = NeteaseParams(
-            url = LYRIC_API,
-            encode_data = self.lyric_encode_data
-        ).get_resource()['lrc']['lyric'].replace("\n", '\n')
+        self.lyric = (
+            NeteaseParams(url=LYRIC_API, encode_data=self.lyric_encode_data)
+            .get_resource()["lrc"]["lyric"]
+            .replace("\n", "\n")
+        )
         # filename = self.get_formated_filename('lrc')
-        filename = self.filename_info['lyric']
-        with open(file = filename, mode = 'w+', encoding = 'UTF-8') as file:
+        filename = self.filename_info["lyric"]
+        with open(file=filename, mode="w+", encoding="UTF-8") as file:
             file.write(self.lyric)
         return filename
 
-    def attribute_write(self, filename = 'No filename'):
-        '''
+    def attribute_write(self, filename="No filename"):
+        """
         往文件里面写入歌曲信息
         ----------
-        参数: 
+        参数:
         1. `filename`: 文件名，字符串，仅mp3/flac格式
-        '''
-        filename_ready = self.get_formated_filename('mp3')
-        if filename == 'No filename':
-            if self.filename_info.get('song') == None:
+        """
+        filename_ready = self.get_formated_filename("mp3")
+        if filename == "No filename":
+            if self.filename_info.get("song") == None:
                 filename = filename_ready
-            else: filename = self.filename_info['song']
-        attribute_write(filename = filename, info = self.processed_info)
+            else:
+                filename = self.filename_info["song"]
+        attribute_write(filename=filename, info=self.processed_info)
 
-    def cover_write(self, filename = 'No filename', cover_filename = 'No cover_filename'):
-        '''
+    def cover_write(self, filename="No filename", cover_filename="No cover_filename"):
+        """
         专辑封面写入
         ----------
-        参数: 
+        参数:
         1. `filename`: 文件名，字符串，仅mp3/flac格式
         2. `cover_filename`: 封面的文件名, 字符串, 仅jpg格式
-        '''
-        if filename == 'No filename':
-            filename = self.filename_info['song']
-        if cover_filename == 'No cover_filename':
-            cover_filename = self.filename_info['pic']
-        cover_write(filename = filename, cover_filename = cover_filename)
-
-    def lyric_write(self, filename = 'No filename', lyric_filename = 'No lyric_filename'):
-        if filename == 'No filename':
-            filename = self.filename_info['song']
-        if lyric_filename == 'No lyric_filename':
-            lyric_filename = self.filename_info['lyric']
-        lyric_write(filename = filename, lyric_filename = lyric_filename)
+        """
+        if filename == "No filename":
+            filename = self.filename_info["song"]
+        if cover_filename == "No cover_filename":
+            cover_filename = self.filename_info["pic"]
+        cover_write(filename=filename, cover_filename=cover_filename)
+
+    def lyric_write(self, filename="No filename", lyric_filename="No lyric_filename"):
+        if filename == "No filename":
+            filename = self.filename_info["song"]
+        if lyric_filename == "No lyric_filename":
+            lyric_filename = self.filename_info["lyric"]
+        lyric_write(filename=filename, lyric_filename=lyric_filename)
 
-    def auto_run(self, d = None):
+    def auto_run(self, d=None):
         self.get_info()
-        if d['song_download'] == True:
+        if d["song_download"] == True:
             c = self.song_download()
             if c == -1:
                 self.is_dl = True
                 return -1
-        if d['cover_download'] == True:
+        if d["cover_download"] == True:
             self.cover_download()
-        if d['lyric_download'] == True:
+        if d["lyric_download"] == True:
             self.lyric_get()
-        if d['attribute_write'] == True:
+        if d["attribute_write"] == True:
             self.attribute_write()
-        if d['cover_write'] == True:
+        if d["cover_write"] == True:
             self.cover_write()
-        if d['lyric_write'] == True:
+        if d["lyric_write"] == True:
             self.lyric_write()
         self.is_dl = True
 
-    def multi_run(self, d = None):
-        threading.Thread(target = self.auto_run, args = (d,)).start()
+    def multi_run(self, d=None):
+        threading.Thread(target=self.auto_run, args=(d,)).start()
```

### Comparing `ncmlistdownloader-1.0.4.240427/ncmlistdownloader.egg-info/PKG-INFO` & `ncmlistdownloader-1.0.5.240429/ncmlistdownloader.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ncmlistdownloader
-Version: 1.0.4.240427
+Version: 1.0.5.240429
 Summary: 获取网易云音乐歌单数据，下载音乐，主动添加元信息。
 Home-page: https://gitee.com/Cooooldwind/163ListDownloader_NexT
 Author: CooooldWind_
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Customer Service
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: End Users/Desktop
```

### Comparing `ncmlistdownloader-1.0.4.240427/ncmlistdownloader.egg-info/SOURCES.txt` & `ncmlistdownloader-1.0.5.240429/ncmlistdownloader.egg-info/SOURCES.txt`

 * *Files identical despite different names*

