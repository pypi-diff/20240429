# Comparing `tmp/python_115-0.0.7.3.tar.gz` & `tmp/python_115-0.0.7.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_115-0.0.7.3.tar", max compression
+gzip compressed data, was "python_115-0.0.7.3.1.tar", max compression
```

## Comparing `python_115-0.0.7.3.tar` & `python_115-0.0.7.3.1.tar`

### file list

```diff
@@ -1,35 +1,35 @@
--rwxr-xr-x   0        0        0     1100 2023-10-11 13:48:41.987287 python_115-0.0.7.3/LICENSE
--rwxr-xr-x   0        0        0   289048 2024-04-29 04:08:16.217988 python_115-0.0.7.3/p115/__init__.py
--rwxr-xr-x   0        0        0      169 2024-04-27 09:40:13.488720 python_115-0.0.7.3/p115/__main__.py
--rwxr-xr-x   0        0        0      161 2024-04-19 14:59:47.539120 python_115-0.0.7.3/p115/cmd/__init__.py
--rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.7.3/p115/cmd/fuse.py
--rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.7.3/p115/cmd/fuse_share.py
--rwxr-xr-x   0        0        0      326 2024-04-27 09:40:34.029692 python_115-0.0.7.3/p115/cmd/init.py
--rwxr-xr-x   0        0        0     8556 2024-04-29 03:49:20.149319 python_115-0.0.7.3/p115/cmd/iterdir.py
--rwxr-xr-x   0        0        0     1837 2024-04-27 13:03:42.950016 python_115-0.0.7.3/p115/cmd/qrcode.py
--rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.7.3/p115/cmd/shell.py
--rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.7.3/p115/cmd/webdav.py
--rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.7.3/p115/cmd/webdav_share.py
--rw-r--r--   0        0        0      179 2023-12-22 08:44:22.766732 python_115-0.0.7.3/p115/exception.py
--rw-r--r--   0        0        0        0 2024-01-30 04:55:37.590943 python_115-0.0.7.3/p115/py.typed
--rwxr-xr-x   0        0        0     3070 2024-04-27 13:16:27.994546 python_115-0.0.7.3/p115/tool/__init__.py
--rw-r--r--   0        0        0       87 2023-12-19 14:25:03.149217 python_115-0.0.7.3/p115/util/__init__.py
--rw-r--r--   0        0        0     4329 2023-11-24 07:50:22.455279 python_115-0.0.7.3/p115/util/_init_mimetypes.py
--rwxr-xr-x   0        0        0      360 2024-04-22 14:19:39.864074 python_115-0.0.7.3/p115/util/args.py
--rw-r--r--   0        0        0     7920 2023-12-14 11:02:29.316261 python_115-0.0.7.3/p115/util/cipher.py
--rw-r--r--   0        0        0     5671 2024-04-03 04:46:18.484632 python_115-0.0.7.3/p115/util/concurrent.py
--rwxr-xr-x   0        0        0    12230 2024-04-25 02:39:02.864829 python_115-0.0.7.3/p115/util/download.py
--rw-r--r--   0        0        0    15103 2024-04-03 05:18:09.304611 python_115-0.0.7.3/p115/util/file.py
--rw-r--r--   0        0        0     4507 2023-12-08 06:07:31.193403 python_115-0.0.7.3/p115/util/hash.py
--rw-r--r--   0        0        0    10070 2024-01-12 05:37:18.775493 python_115-0.0.7.3/p115/util/ignore.py
--rw-r--r--   0        0        0     2822 2024-02-13 03:37:52.593362 python_115-0.0.7.3/p115/util/iter.py
--rw-r--r--   0        0        0     4562 2024-01-16 05:10:10.057134 python_115-0.0.7.3/p115/util/path.py
--rwxr-xr-x   0        0        0     1846 2024-04-24 15:33:36.222174 python_115-0.0.7.3/p115/util/property.py
--rw-r--r--   0        0        0     3190 2024-01-29 10:59:02.879730 python_115-0.0.7.3/p115/util/response.py
--rwxr-xr-x   0        0        0     6150 2024-04-24 16:05:44.697816 python_115-0.0.7.3/p115/util/retry.py
--rw-r--r--   0        0        0     6785 2024-02-09 07:54:09.097617 python_115-0.0.7.3/p115/util/text.py
--rw-r--r--   0        0        0       43 2024-04-03 05:08:27.538028 python_115-0.0.7.3/p115/util/upload.py
--rw-r--r--   0        0        0    10029 2024-01-29 10:52:22.271824 python_115-0.0.7.3/p115/util/urlopen.py
--rw-r--r--   0        0        0     1272 2024-04-29 04:08:51.598357 python_115-0.0.7.3/pyproject.toml
--rw-r--r--   0        0        0    34641 2024-01-05 10:56:58.191328 python_115-0.0.7.3/readme.md
--rw-r--r--   0        0        0    35896 1970-01-01 00:00:00.000000 python_115-0.0.7.3/PKG-INFO
+-rwxr-xr-x   0        0        0     1100 2023-10-11 13:48:41.987287 python_115-0.0.7.3.1/LICENSE
+-rwxr-xr-x   0        0        0   289049 2024-04-29 04:13:19.201786 python_115-0.0.7.3.1/p115/__init__.py
+-rwxr-xr-x   0        0        0      169 2024-04-27 09:40:13.488720 python_115-0.0.7.3.1/p115/__main__.py
+-rwxr-xr-x   0        0        0      161 2024-04-19 14:59:47.539120 python_115-0.0.7.3.1/p115/cmd/__init__.py
+-rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.7.3.1/p115/cmd/fuse.py
+-rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.7.3.1/p115/cmd/fuse_share.py
+-rwxr-xr-x   0        0        0      326 2024-04-27 09:40:34.029692 python_115-0.0.7.3.1/p115/cmd/init.py
+-rwxr-xr-x   0        0        0     8556 2024-04-29 03:49:20.149319 python_115-0.0.7.3.1/p115/cmd/iterdir.py
+-rwxr-xr-x   0        0        0     1837 2024-04-27 13:03:42.950016 python_115-0.0.7.3.1/p115/cmd/qrcode.py
+-rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.7.3.1/p115/cmd/shell.py
+-rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.7.3.1/p115/cmd/webdav.py
+-rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.7.3.1/p115/cmd/webdav_share.py
+-rw-r--r--   0        0        0      179 2023-12-22 08:44:22.766732 python_115-0.0.7.3.1/p115/exception.py
+-rw-r--r--   0        0        0        0 2024-01-30 04:55:37.590943 python_115-0.0.7.3.1/p115/py.typed
+-rwxr-xr-x   0        0        0     3070 2024-04-27 13:16:27.994546 python_115-0.0.7.3.1/p115/tool/__init__.py
+-rw-r--r--   0        0        0       87 2023-12-19 14:25:03.149217 python_115-0.0.7.3.1/p115/util/__init__.py
+-rw-r--r--   0        0        0     4329 2023-11-24 07:50:22.455279 python_115-0.0.7.3.1/p115/util/_init_mimetypes.py
+-rwxr-xr-x   0        0        0      360 2024-04-22 14:19:39.864074 python_115-0.0.7.3.1/p115/util/args.py
+-rw-r--r--   0        0        0     7920 2023-12-14 11:02:29.316261 python_115-0.0.7.3.1/p115/util/cipher.py
+-rw-r--r--   0        0        0     5671 2024-04-03 04:46:18.484632 python_115-0.0.7.3.1/p115/util/concurrent.py
+-rwxr-xr-x   0        0        0    12230 2024-04-25 02:39:02.864829 python_115-0.0.7.3.1/p115/util/download.py
+-rw-r--r--   0        0        0    15103 2024-04-03 05:18:09.304611 python_115-0.0.7.3.1/p115/util/file.py
+-rw-r--r--   0        0        0     4507 2023-12-08 06:07:31.193403 python_115-0.0.7.3.1/p115/util/hash.py
+-rw-r--r--   0        0        0    10070 2024-01-12 05:37:18.775493 python_115-0.0.7.3.1/p115/util/ignore.py
+-rw-r--r--   0        0        0     2822 2024-02-13 03:37:52.593362 python_115-0.0.7.3.1/p115/util/iter.py
+-rw-r--r--   0        0        0     4562 2024-01-16 05:10:10.057134 python_115-0.0.7.3.1/p115/util/path.py
+-rwxr-xr-x   0        0        0     1846 2024-04-24 15:33:36.222174 python_115-0.0.7.3.1/p115/util/property.py
+-rw-r--r--   0        0        0     3190 2024-01-29 10:59:02.879730 python_115-0.0.7.3.1/p115/util/response.py
+-rwxr-xr-x   0        0        0     6150 2024-04-24 16:05:44.697816 python_115-0.0.7.3.1/p115/util/retry.py
+-rw-r--r--   0        0        0     6785 2024-02-09 07:54:09.097617 python_115-0.0.7.3.1/p115/util/text.py
+-rw-r--r--   0        0        0       43 2024-04-03 05:08:27.538028 python_115-0.0.7.3.1/p115/util/upload.py
+-rw-r--r--   0        0        0    10029 2024-01-29 10:52:22.271824 python_115-0.0.7.3.1/p115/util/urlopen.py
+-rw-r--r--   0        0        0     1274 2024-04-29 04:13:36.461812 python_115-0.0.7.3.1/pyproject.toml
+-rw-r--r--   0        0        0    34641 2024-01-05 10:56:58.191328 python_115-0.0.7.3.1/readme.md
+-rw-r--r--   0        0        0    35898 1970-01-01 00:00:00.000000 python_115-0.0.7.3.1/PKG-INFO
```

### Comparing `python_115-0.0.7.3/LICENSE` & `python_115-0.0.7.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `python_115-0.0.7.3/p115/__init__.py` & `python_115-0.0.7.3.1/p115/__init__.py`

 * *Files identical despite different names*

```diff
@@ -130,15 +130,15 @@
                 # {'state': False, 'error': '复制[...]操作尚未执行完成，请稍后再试！', 'errno': 990009, 'errtype': 'war'}
                 # {'state': False, 'error': '移动[...]操作尚未执行完成，请稍后再试！', 'errno': 990009, 'errtype': 'war'}
                 case 990009:
                     raise OSError(errno.EBUSY, resp)
                 # {'state': False, 'error': '操作的文件(夹)数量超过5万个', 'errno': 990023, 'errtype': ''}
                 case 990023:
                     raise OSError(errno.ENOTSUP, resp)
-            raise OSError(errno.EIO, resp)
+        raise OSError(errno.EIO, resp)
     if isinstance(fn, dict):
         return check(fn)
     elif iscoroutinefunction(fn):
         async def wrapper(*args, **kwds):
             return check(await fn(*args, **kwds))
     elif callable(fn):
         def wrapper(*args, **kwds):
@@ -1318,15 +1318,15 @@
     ) -> ExportDirStatus:
         """执行导出目录树，新开启一个线程，用于检查完成状态
         payload:
             file_ids: int | str   # 有多个时，用逗号 "," 隔开
             target: str = "U_1_0" # 导出目录树到这个目录
             layer_limit: int = <default> # 层级深度，自然数
         """
-        resp = check_response(self.fs_export_dir(payload, async_=async_, **request_kwargs))
+        resp = self.fs_export_dir(payload, async_=async_, **request_kwargs)
         return ExportDirStatus(self, resp["data"]["export_id"])
 
     def fs_shortcut_get(
         self, 
         payload: int | str | dict, 
         /, 
         async_: bool = False, 
@@ -6583,14 +6583,15 @@
                 return False
             hidden = not show
             check_response(self.client.fs_files_hidden({"hidden": int(hidden), "fid[0]": fid}))
             return hidden
 
     @property
     def hidden_mode(self, /) -> bool:
+        breakpoint()
         return check_response(self.client.user_setting())["data"]["show"] == "1"
 
     def hidden_switch(
         self, 
         /, 
         show: None | bool = None, 
         password: str = "",
```

### Comparing `python_115-0.0.7.3/p115/cmd/iterdir.py` & `python_115-0.0.7.3.1/p115/cmd/iterdir.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.7.3/p115/cmd/qrcode.py` & `python_115-0.0.7.3.1/p115/cmd/qrcode.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.7.3/p115/tool/__init__.py` & `python_115-0.0.7.3.1/p115/tool/__init__.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.7.3/p115/util/_init_mimetypes.py` & `python_115-0.0.7.3.1/p115/util/_init_mimetypes.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.7.3/p115/util/cipher.py` & `python_115-0.0.7.3.1/p115/util/cipher.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.7.3/p115/util/concurrent.py` & `python_115-0.0.7.3.1/p115/util/concurrent.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.7.3/p115/util/download.py` & `python_115-0.0.7.3.1/p115/util/download.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.7.3/p115/util/file.py` & `python_115-0.0.7.3.1/p115/util/file.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.7.3/p115/util/hash.py` & `python_115-0.0.7.3.1/p115/util/hash.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.7.3/p115/util/ignore.py` & `python_115-0.0.7.3.1/p115/util/ignore.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.7.3/p115/util/iter.py` & `python_115-0.0.7.3.1/p115/util/iter.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.7.3/p115/util/path.py` & `python_115-0.0.7.3.1/p115/util/path.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.7.3/p115/util/property.py` & `python_115-0.0.7.3.1/p115/util/property.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.7.3/p115/util/response.py` & `python_115-0.0.7.3.1/p115/util/response.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.7.3/p115/util/retry.py` & `python_115-0.0.7.3.1/p115/util/retry.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.7.3/p115/util/text.py` & `python_115-0.0.7.3.1/p115/util/text.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.7.3/p115/util/urlopen.py` & `python_115-0.0.7.3.1/p115/util/urlopen.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.7.3/pyproject.toml` & `python_115-0.0.7.3.1/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "python-115"
-version = "0.0.7.3"
+version = "0.0.7.3.1"
 description = "Python wrapper for 115 webdisk."
 authors = ["ChenyangGao <wosiwujm@gmail.com>"]
 license = "MIT"
 readme = "readme.md"
 homepage = "https://github.com/ChenyangGao/web-mount-packs/tree/main/python-115-client"
 repository = "https://github.com/ChenyangGao/web-mount-packs/tree/main/python-115-client"
 keywords = ["nas", "115"]
```

### Comparing `python_115-0.0.7.3/readme.md` & `python_115-0.0.7.3.1/readme.md`

 * *Files identical despite different names*

### Comparing `python_115-0.0.7.3/PKG-INFO` & `python_115-0.0.7.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-115
-Version: 0.0.7.3
+Version: 0.0.7.3.1
 Summary: Python wrapper for 115 webdisk.
 Home-page: https://github.com/ChenyangGao/web-mount-packs/tree/main/python-115-client
 License: MIT
 Keywords: nas,115
 Author: ChenyangGao
 Author-email: wosiwujm@gmail.com
 Requires-Python: >=3.11,<4.0
```

