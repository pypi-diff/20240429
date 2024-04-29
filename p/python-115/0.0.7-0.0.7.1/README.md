# Comparing `tmp/python_115-0.0.7.tar.gz` & `tmp/python_115-0.0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_115-0.0.7.tar", max compression
+gzip compressed data, was "python_115-0.0.7.1.tar", max compression
```

## Comparing `python_115-0.0.7.tar` & `python_115-0.0.7.1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rwxr-xr-x   0        0        0     1100 2023-10-11 13:48:41.987287 python_115-0.0.7/LICENSE
--rwxr-xr-x   0        0        0   287484 2024-04-28 15:43:44.390863 python_115-0.0.7/p115/__init__.py
--rwxr-xr-x   0        0        0      169 2024-04-27 09:40:13.488720 python_115-0.0.7/p115/__main__.py
--rwxr-xr-x   0        0        0      161 2024-04-19 14:59:47.539120 python_115-0.0.7/p115/cmd/__init__.py
--rwxr-xr-x   0        0        0      326 2024-04-27 09:40:34.029692 python_115-0.0.7/p115/cmd/init.py
--rwxr-xr-x   0        0        0     6857 2024-04-28 15:44:22.845020 python_115-0.0.7/p115/cmd/iterdir.py
--rwxr-xr-x   0        0        0     1837 2024-04-27 13:03:42.950016 python_115-0.0.7/p115/cmd/qrcode.py
--rw-r--r--   0        0        0      179 2023-12-22 08:44:22.766732 python_115-0.0.7/p115/exception.py
--rw-r--r--   0        0        0        0 2024-01-30 04:55:37.590943 python_115-0.0.7/p115/py.typed
--rwxr-xr-x   0        0        0     3070 2024-04-27 13:16:27.994546 python_115-0.0.7/p115/tool/__init__.py
--rw-r--r--   0        0        0       87 2023-12-19 14:25:03.149217 python_115-0.0.7/p115/util/__init__.py
--rw-r--r--   0        0        0     4329 2023-11-24 07:50:22.455279 python_115-0.0.7/p115/util/_init_mimetypes.py
--rwxr-xr-x   0        0        0      360 2024-04-22 14:19:39.864074 python_115-0.0.7/p115/util/args.py
--rw-r--r--   0        0        0     7920 2023-12-14 11:02:29.316261 python_115-0.0.7/p115/util/cipher.py
--rw-r--r--   0        0        0     5671 2024-04-03 04:46:18.484632 python_115-0.0.7/p115/util/concurrent.py
--rwxr-xr-x   0        0        0    12230 2024-04-25 02:39:02.864829 python_115-0.0.7/p115/util/download.py
--rw-r--r--   0        0        0    15103 2024-04-03 05:18:09.304611 python_115-0.0.7/p115/util/file.py
--rw-r--r--   0        0        0     4507 2023-12-08 06:07:31.193403 python_115-0.0.7/p115/util/hash.py
--rw-r--r--   0        0        0    10070 2024-01-12 05:37:18.775493 python_115-0.0.7/p115/util/ignore.py
--rw-r--r--   0        0        0     2822 2024-02-13 03:37:52.593362 python_115-0.0.7/p115/util/iter.py
--rw-r--r--   0        0        0     4562 2024-01-16 05:10:10.057134 python_115-0.0.7/p115/util/path.py
--rwxr-xr-x   0        0        0     1846 2024-04-24 15:33:36.222174 python_115-0.0.7/p115/util/property.py
--rw-r--r--   0        0        0     3190 2024-01-29 10:59:02.879730 python_115-0.0.7/p115/util/response.py
--rwxr-xr-x   0        0        0     6150 2024-04-24 16:05:44.697816 python_115-0.0.7/p115/util/retry.py
--rw-r--r--   0        0        0     6785 2024-02-09 07:54:09.097617 python_115-0.0.7/p115/util/text.py
--rw-r--r--   0        0        0       43 2024-04-03 05:08:27.538028 python_115-0.0.7/p115/util/upload.py
--rw-r--r--   0        0        0    10029 2024-01-29 10:52:22.271824 python_115-0.0.7/p115/util/urlopen.py
--rw-r--r--   0        0        0     1270 2024-04-28 14:00:49.525373 python_115-0.0.7/pyproject.toml
--rw-r--r--   0        0        0    34641 2024-01-05 10:56:58.191328 python_115-0.0.7/readme.md
--rw-r--r--   0        0        0    35894 1970-01-01 00:00:00.000000 python_115-0.0.7/PKG-INFO
+-rwxr-xr-x   0        0        0     1100 2023-10-11 13:48:41.987287 python_115-0.0.7.1/LICENSE
+-rwxr-xr-x   0        0        0   287500 2024-04-28 16:00:30.281254 python_115-0.0.7.1/p115/__init__.py
+-rwxr-xr-x   0        0        0      169 2024-04-27 09:40:13.488720 python_115-0.0.7.1/p115/__main__.py
+-rwxr-xr-x   0        0        0      161 2024-04-19 14:59:47.539120 python_115-0.0.7.1/p115/cmd/__init__.py
+-rwxr-xr-x   0        0        0      326 2024-04-27 09:40:34.029692 python_115-0.0.7.1/p115/cmd/init.py
+-rwxr-xr-x   0        0        0     7038 2024-04-28 15:59:13.863161 python_115-0.0.7.1/p115/cmd/iterdir.py
+-rwxr-xr-x   0        0        0     1837 2024-04-27 13:03:42.950016 python_115-0.0.7.1/p115/cmd/qrcode.py
+-rw-r--r--   0        0        0      179 2023-12-22 08:44:22.766732 python_115-0.0.7.1/p115/exception.py
+-rw-r--r--   0        0        0        0 2024-01-30 04:55:37.590943 python_115-0.0.7.1/p115/py.typed
+-rwxr-xr-x   0        0        0     3070 2024-04-27 13:16:27.994546 python_115-0.0.7.1/p115/tool/__init__.py
+-rw-r--r--   0        0        0       87 2023-12-19 14:25:03.149217 python_115-0.0.7.1/p115/util/__init__.py
+-rw-r--r--   0        0        0     4329 2023-11-24 07:50:22.455279 python_115-0.0.7.1/p115/util/_init_mimetypes.py
+-rwxr-xr-x   0        0        0      360 2024-04-22 14:19:39.864074 python_115-0.0.7.1/p115/util/args.py
+-rw-r--r--   0        0        0     7920 2023-12-14 11:02:29.316261 python_115-0.0.7.1/p115/util/cipher.py
+-rw-r--r--   0        0        0     5671 2024-04-03 04:46:18.484632 python_115-0.0.7.1/p115/util/concurrent.py
+-rwxr-xr-x   0        0        0    12230 2024-04-25 02:39:02.864829 python_115-0.0.7.1/p115/util/download.py
+-rw-r--r--   0        0        0    15103 2024-04-03 05:18:09.304611 python_115-0.0.7.1/p115/util/file.py
+-rw-r--r--   0        0        0     4507 2023-12-08 06:07:31.193403 python_115-0.0.7.1/p115/util/hash.py
+-rw-r--r--   0        0        0    10070 2024-01-12 05:37:18.775493 python_115-0.0.7.1/p115/util/ignore.py
+-rw-r--r--   0        0        0     2822 2024-02-13 03:37:52.593362 python_115-0.0.7.1/p115/util/iter.py
+-rw-r--r--   0        0        0     4562 2024-01-16 05:10:10.057134 python_115-0.0.7.1/p115/util/path.py
+-rwxr-xr-x   0        0        0     1846 2024-04-24 15:33:36.222174 python_115-0.0.7.1/p115/util/property.py
+-rw-r--r--   0        0        0     3190 2024-01-29 10:59:02.879730 python_115-0.0.7.1/p115/util/response.py
+-rwxr-xr-x   0        0        0     6150 2024-04-24 16:05:44.697816 python_115-0.0.7.1/p115/util/retry.py
+-rw-r--r--   0        0        0     6785 2024-02-09 07:54:09.097617 python_115-0.0.7.1/p115/util/text.py
+-rw-r--r--   0        0        0       43 2024-04-03 05:08:27.538028 python_115-0.0.7.1/p115/util/upload.py
+-rw-r--r--   0        0        0    10029 2024-01-29 10:52:22.271824 python_115-0.0.7.1/p115/util/urlopen.py
+-rw-r--r--   0        0        0     1272 2024-04-28 16:00:46.494910 python_115-0.0.7.1/pyproject.toml
+-rw-r--r--   0        0        0    34641 2024-01-05 10:56:58.191328 python_115-0.0.7.1/readme.md
+-rw-r--r--   0        0        0    35896 1970-01-01 00:00:00.000000 python_115-0.0.7.1/PKG-INFO
```

### Comparing `python_115-0.0.7/LICENSE` & `python_115-0.0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `python_115-0.0.7/p115/__init__.py` & `python_115-0.0.7.1/p115/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from __future__ import annotations
 
 __author__ = "ChenyangGao <https://chenyanggao.github.io>"
 __version__ = (0, 0, 7)
 __all__ = [
     "P115Client", "P115Path", "P115FileSystem", "P115SharePath", "P115ShareFileSystem", 
     "P115ZipPath", "P115ZipFileSystem", "P115Offline", "P115Recyclebin", "P115Sharing", 
-    "LabelList", 
+    "P115LabelList", 
 ]
 
 import errno
 
 from abc import ABC, abstractmethod
 from asyncio import get_running_loop, run_coroutine_threadsafe, run, to_thread
 from binascii import b2a_hex
@@ -4052,18 +4052,18 @@
 
     def get_zip_fs(self, id_or_pickcode: int | str, /, *args, **kwargs) -> P115ZipFileSystem:
         """
         """
         return P115ZipFileSystem(self, id_or_pickcode, *args, **kwargs)
 
     @cached_property
-    def label(self, /) -> LabelList:
+    def label(self, /) -> P115LabelList:
         """
         """
-        return LabelList(self)
+        return P115LabelList(self)
 
     @cached_property
     def offline(self, /) -> P115Offline:
         """
         """
         return P115Offline(self)
 
@@ -8221,15 +8221,15 @@
         })
 
     @check_response
     def update(self, /, share_code: str, **payload) -> dict:
         return self.client.share_update({"share_code": share_code, **payload})
 
 
-class LabelList:
+class P115LabelList:
     __slots__ = "client",
 
     def __init__(self, client: P115Client, /):
         self.client = client
 
     def __contains__(self, id_or_name: int | str, /) -> bool:
         if isinstance(id_or_name, int):
```

### Comparing `python_115-0.0.7/p115/cmd/iterdir.py` & `python_115-0.0.7.1/p115/cmd/iterdir.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,14 +42,17 @@
             except FileNotFoundError:
                 pass
 
     fs = P115FileSystem.login(cookie)
     if fs.client.cookie != cookie:
         open("115-cookie.txt", "w").write(fs.client.cookie)
 
+    if args.password:
+        fs.hidden_switch(True, password=args.password)
+
     keys = args.keys or KEYS
     output_type = args.output_type
 
     path = args.path
     if path.isdecimal():
         fid = int(path)
     else:
@@ -163,14 +166,15 @@
         stderr.close()
     finally:
         file.close()
 
 
 parser.add_argument("path", nargs="?", default="0", help="文件夹路径或 id，默认值 0，即根目录")
 parser.add_argument("-c", "--cookie", help="115 登录 cookie，如果缺失，则从 115-cookie.txt 文件中获取，此文件可以在 当前工作目录、此脚本所在目录 或 用户根目录 下")
+parser.add_argument("-p", "--password", help="密码，用于进入隐藏模式，罗列隐藏文件")
 parser.add_argument("-k", "--keys", nargs="*", choices=KEYS, help=f"选择输出的 key，默认输出所有可选值")
 parser.add_argument("-s", "--select", help="提供一个表达式（会注入一个变量 path，类型是 p115.P115Path），用于对路径进行筛选")
 parser.add_argument("-t", "--output-type", choices=("log", "json", "csv"), default="log", help="""
 输出类型，默认为 log
 - log   每行输出一条数据，每条数据输出为一个 json 的 object
 - json  输出一个 json 的 list，每条数据输出为一个 json 的 object
 - csv   输出一个 csv，第 1 行为表头，以后每行输出一条数据
```

### Comparing `python_115-0.0.7/p115/cmd/qrcode.py` & `python_115-0.0.7.1/p115/cmd/qrcode.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.7/p115/tool/__init__.py` & `python_115-0.0.7.1/p115/tool/__init__.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.7/p115/util/_init_mimetypes.py` & `python_115-0.0.7.1/p115/util/_init_mimetypes.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.7/p115/util/cipher.py` & `python_115-0.0.7.1/p115/util/cipher.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.7/p115/util/concurrent.py` & `python_115-0.0.7.1/p115/util/concurrent.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.7/p115/util/download.py` & `python_115-0.0.7.1/p115/util/download.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.7/p115/util/file.py` & `python_115-0.0.7.1/p115/util/file.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.7/p115/util/hash.py` & `python_115-0.0.7.1/p115/util/hash.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.7/p115/util/ignore.py` & `python_115-0.0.7.1/p115/util/ignore.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.7/p115/util/iter.py` & `python_115-0.0.7.1/p115/util/iter.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.7/p115/util/path.py` & `python_115-0.0.7.1/p115/util/path.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.7/p115/util/property.py` & `python_115-0.0.7.1/p115/util/property.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.7/p115/util/response.py` & `python_115-0.0.7.1/p115/util/response.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.7/p115/util/retry.py` & `python_115-0.0.7.1/p115/util/retry.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.7/p115/util/text.py` & `python_115-0.0.7.1/p115/util/text.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.7/p115/util/urlopen.py` & `python_115-0.0.7.1/p115/util/urlopen.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.7/pyproject.toml` & `python_115-0.0.7.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "python-115"
-version = "0.0.7"
+version = "0.0.7.1"
 description = "Python wrapper for 115 webdisk."
 authors = ["ChenyangGao <wosiwujm@gmail.com>"]
 license = "MIT"
 readme = "readme.md"
 homepage = "https://github.com/ChenyangGao/web-mount-packs/tree/main/python-115-client"
 repository = "https://github.com/ChenyangGao/web-mount-packs/tree/main/python-115-client"
 keywords = ["nas", "115"]
```

### Comparing `python_115-0.0.7/readme.md` & `python_115-0.0.7.1/readme.md`

 * *Files identical despite different names*

### Comparing `python_115-0.0.7/PKG-INFO` & `python_115-0.0.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-115
-Version: 0.0.7
+Version: 0.0.7.1
 Summary: Python wrapper for 115 webdisk.
 Home-page: https://github.com/ChenyangGao/web-mount-packs/tree/main/python-115-client
 License: MIT
 Keywords: nas,115
 Author: ChenyangGao
 Author-email: wosiwujm@gmail.com
 Requires-Python: >=3.11,<4.0
```

