# Comparing `tmp/python_115-0.0.7.2.tar.gz` & `tmp/python_115-0.0.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_115-0.0.7.2.tar", max compression
+gzip compressed data, was "python_115-0.0.7.3.tar", max compression
```

## Comparing `python_115-0.0.7.2.tar` & `python_115-0.0.7.3.tar`

### file list

```diff
@@ -1,35 +1,35 @@
--rwxr-xr-x   0        0        0     1100 2023-10-11 13:48:41.987287 python_115-0.0.7.2/LICENSE
--rwxr-xr-x   0        0        0   287661 2024-04-29 01:47:06.716348 python_115-0.0.7.2/p115/__init__.py
--rwxr-xr-x   0        0        0      169 2024-04-27 09:40:13.488720 python_115-0.0.7.2/p115/__main__.py
--rwxr-xr-x   0        0        0      161 2024-04-19 14:59:47.539120 python_115-0.0.7.2/p115/cmd/__init__.py
--rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.7.2/p115/cmd/fuse.py
--rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.7.2/p115/cmd/fuse_share.py
--rwxr-xr-x   0        0        0      326 2024-04-27 09:40:34.029692 python_115-0.0.7.2/p115/cmd/init.py
--rwxr-xr-x   0        0        0     7038 2024-04-28 15:59:13.863161 python_115-0.0.7.2/p115/cmd/iterdir.py
--rwxr-xr-x   0        0        0     1837 2024-04-27 13:03:42.950016 python_115-0.0.7.2/p115/cmd/qrcode.py
--rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.7.2/p115/cmd/shell.py
--rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.7.2/p115/cmd/webdav.py
--rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.7.2/p115/cmd/webdav_share.py
--rw-r--r--   0        0        0      179 2023-12-22 08:44:22.766732 python_115-0.0.7.2/p115/exception.py
--rw-r--r--   0        0        0        0 2024-01-30 04:55:37.590943 python_115-0.0.7.2/p115/py.typed
--rwxr-xr-x   0        0        0     3070 2024-04-27 13:16:27.994546 python_115-0.0.7.2/p115/tool/__init__.py
--rw-r--r--   0        0        0       87 2023-12-19 14:25:03.149217 python_115-0.0.7.2/p115/util/__init__.py
--rw-r--r--   0        0        0     4329 2023-11-24 07:50:22.455279 python_115-0.0.7.2/p115/util/_init_mimetypes.py
--rwxr-xr-x   0        0        0      360 2024-04-22 14:19:39.864074 python_115-0.0.7.2/p115/util/args.py
--rw-r--r--   0        0        0     7920 2023-12-14 11:02:29.316261 python_115-0.0.7.2/p115/util/cipher.py
--rw-r--r--   0        0        0     5671 2024-04-03 04:46:18.484632 python_115-0.0.7.2/p115/util/concurrent.py
--rwxr-xr-x   0        0        0    12230 2024-04-25 02:39:02.864829 python_115-0.0.7.2/p115/util/download.py
--rw-r--r--   0        0        0    15103 2024-04-03 05:18:09.304611 python_115-0.0.7.2/p115/util/file.py
--rw-r--r--   0        0        0     4507 2023-12-08 06:07:31.193403 python_115-0.0.7.2/p115/util/hash.py
--rw-r--r--   0        0        0    10070 2024-01-12 05:37:18.775493 python_115-0.0.7.2/p115/util/ignore.py
--rw-r--r--   0        0        0     2822 2024-02-13 03:37:52.593362 python_115-0.0.7.2/p115/util/iter.py
--rw-r--r--   0        0        0     4562 2024-01-16 05:10:10.057134 python_115-0.0.7.2/p115/util/path.py
--rwxr-xr-x   0        0        0     1846 2024-04-24 15:33:36.222174 python_115-0.0.7.2/p115/util/property.py
--rw-r--r--   0        0        0     3190 2024-01-29 10:59:02.879730 python_115-0.0.7.2/p115/util/response.py
--rwxr-xr-x   0        0        0     6150 2024-04-24 16:05:44.697816 python_115-0.0.7.2/p115/util/retry.py
--rw-r--r--   0        0        0     6785 2024-02-09 07:54:09.097617 python_115-0.0.7.2/p115/util/text.py
--rw-r--r--   0        0        0       43 2024-04-03 05:08:27.538028 python_115-0.0.7.2/p115/util/upload.py
--rw-r--r--   0        0        0    10029 2024-01-29 10:52:22.271824 python_115-0.0.7.2/p115/util/urlopen.py
--rw-r--r--   0        0        0     1272 2024-04-29 01:47:40.043085 python_115-0.0.7.2/pyproject.toml
--rw-r--r--   0        0        0    34641 2024-01-05 10:56:58.191328 python_115-0.0.7.2/readme.md
--rw-r--r--   0        0        0    35896 1970-01-01 00:00:00.000000 python_115-0.0.7.2/PKG-INFO
+-rwxr-xr-x   0        0        0     1100 2023-10-11 13:48:41.987287 python_115-0.0.7.3/LICENSE
+-rwxr-xr-x   0        0        0   289048 2024-04-29 04:08:16.217988 python_115-0.0.7.3/p115/__init__.py
+-rwxr-xr-x   0        0        0      169 2024-04-27 09:40:13.488720 python_115-0.0.7.3/p115/__main__.py
+-rwxr-xr-x   0        0        0      161 2024-04-19 14:59:47.539120 python_115-0.0.7.3/p115/cmd/__init__.py
+-rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.7.3/p115/cmd/fuse.py
+-rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.7.3/p115/cmd/fuse_share.py
+-rwxr-xr-x   0        0        0      326 2024-04-27 09:40:34.029692 python_115-0.0.7.3/p115/cmd/init.py
+-rwxr-xr-x   0        0        0     8556 2024-04-29 03:49:20.149319 python_115-0.0.7.3/p115/cmd/iterdir.py
+-rwxr-xr-x   0        0        0     1837 2024-04-27 13:03:42.950016 python_115-0.0.7.3/p115/cmd/qrcode.py
+-rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.7.3/p115/cmd/shell.py
+-rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.7.3/p115/cmd/webdav.py
+-rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.7.3/p115/cmd/webdav_share.py
+-rw-r--r--   0        0        0      179 2023-12-22 08:44:22.766732 python_115-0.0.7.3/p115/exception.py
+-rw-r--r--   0        0        0        0 2024-01-30 04:55:37.590943 python_115-0.0.7.3/p115/py.typed
+-rwxr-xr-x   0        0        0     3070 2024-04-27 13:16:27.994546 python_115-0.0.7.3/p115/tool/__init__.py
+-rw-r--r--   0        0        0       87 2023-12-19 14:25:03.149217 python_115-0.0.7.3/p115/util/__init__.py
+-rw-r--r--   0        0        0     4329 2023-11-24 07:50:22.455279 python_115-0.0.7.3/p115/util/_init_mimetypes.py
+-rwxr-xr-x   0        0        0      360 2024-04-22 14:19:39.864074 python_115-0.0.7.3/p115/util/args.py
+-rw-r--r--   0        0        0     7920 2023-12-14 11:02:29.316261 python_115-0.0.7.3/p115/util/cipher.py
+-rw-r--r--   0        0        0     5671 2024-04-03 04:46:18.484632 python_115-0.0.7.3/p115/util/concurrent.py
+-rwxr-xr-x   0        0        0    12230 2024-04-25 02:39:02.864829 python_115-0.0.7.3/p115/util/download.py
+-rw-r--r--   0        0        0    15103 2024-04-03 05:18:09.304611 python_115-0.0.7.3/p115/util/file.py
+-rw-r--r--   0        0        0     4507 2023-12-08 06:07:31.193403 python_115-0.0.7.3/p115/util/hash.py
+-rw-r--r--   0        0        0    10070 2024-01-12 05:37:18.775493 python_115-0.0.7.3/p115/util/ignore.py
+-rw-r--r--   0        0        0     2822 2024-02-13 03:37:52.593362 python_115-0.0.7.3/p115/util/iter.py
+-rw-r--r--   0        0        0     4562 2024-01-16 05:10:10.057134 python_115-0.0.7.3/p115/util/path.py
+-rwxr-xr-x   0        0        0     1846 2024-04-24 15:33:36.222174 python_115-0.0.7.3/p115/util/property.py
+-rw-r--r--   0        0        0     3190 2024-01-29 10:59:02.879730 python_115-0.0.7.3/p115/util/response.py
+-rwxr-xr-x   0        0        0     6150 2024-04-24 16:05:44.697816 python_115-0.0.7.3/p115/util/retry.py
+-rw-r--r--   0        0        0     6785 2024-02-09 07:54:09.097617 python_115-0.0.7.3/p115/util/text.py
+-rw-r--r--   0        0        0       43 2024-04-03 05:08:27.538028 python_115-0.0.7.3/p115/util/upload.py
+-rw-r--r--   0        0        0    10029 2024-01-29 10:52:22.271824 python_115-0.0.7.3/p115/util/urlopen.py
+-rw-r--r--   0        0        0     1272 2024-04-29 04:08:51.598357 python_115-0.0.7.3/pyproject.toml
+-rw-r--r--   0        0        0    34641 2024-01-05 10:56:58.191328 python_115-0.0.7.3/readme.md
+-rw-r--r--   0        0        0    35896 1970-01-01 00:00:00.000000 python_115-0.0.7.3/PKG-INFO
```

### Comparing `python_115-0.0.7.2/LICENSE` & `python_115-0.0.7.3/LICENSE`

 * *Files identical despite different names*

### Comparing `python_115-0.0.7.2/p115/__init__.py` & `python_115-0.0.7.3/p115/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1129,22 +1129,28 @@
     def fs_get_repeat(
         self, 
         payload: int | str | dict, 
         /, 
         async_: bool = False, 
         **request_kwargs, 
     ) -> dict:
-        """文件查重（罗列除此以外的 sha1 相同的文件）
+        """查找重复文件（罗列除此以外的 sha1 相同的文件）
         GET https://webapi.115.com/files/get_repeat_sha
         payload:
             file_id: int | str
+            offset: int = 0
+            limit: int = 1150
+            source: str = ""
+            format: str = "json"
         """
         api = "https://webapi.115.com/files/get_repeat_sha"
         if isinstance(payload, (int, str)):
-            payload = {"file_id": payload}
+            payload = {"offset": 0, "limit": 1150, "format": "json", "file_id": payload}
+        else:
+            payload = {"offset": 0, "limit": 1150, "format": "json", **payload}
         return self.request(api, params=payload, async_=async_, **request_kwargs)
 
     def fs_index_info(
         self, 
         /, 
         async_: bool = False, 
         **request_kwargs, 
@@ -4811,15 +4817,15 @@
             task.run()
         elif submit:
             task.run_wait()
         return task
 
     def download_tree(
         self, 
-        id_or_path: IDOrPathType, 
+        id_or_path: IDOrPathType = "", 
         /, 
         local_dir: bytes | str | PathLike = "", 
         pid: Optional[int] = None, 
         write_mode: Literal["i", "x", "w", "a"] = "a", 
         submit: None | bool | Callable[[Callable], Any] = None, 
         no_root: bool = False, 
         predicate: Optional[Callable[[P115PathType], bool]] = None, 
@@ -6575,19 +6581,26 @@
             fid = self.get_id(id_or_path, pid)
             if fid == 0:
                 return False
             hidden = not show
             check_response(self.client.fs_files_hidden({"hidden": int(hidden), "fid[0]": fid}))
             return hidden
 
+    @property
+    def hidden_mode(self, /) -> bool:
+        return check_response(self.client.user_setting())["data"]["show"] == "1"
+
     def hidden_switch(
         self, 
-        show: bool = True, 
+        /, 
+        show: None | bool = None, 
         password: str = "", 
     ):
+        if show is None:
+            show = not self.hidden_mode
         check_response(self.client.fs_hidden_switch({"show": int(show), "safe_pwd": password or self.password}))
 
     def is_empty(
         self, 
         id_or_path: IDOrPathType = "", 
         /, 
         pid: Optional[int] = None, 
@@ -6600,14 +6613,36 @@
                 attr = self.attr(id_or_path, pid)
             except FileNotFoundError:
                 return True
         if attr["is_directory"]:
             return self.get_directory_capacity(attr["id"]) > 0
         return attr["size"] == 0
 
+    def iter_repeat(
+        self, 
+        id_or_path: IDOrPathType, 
+        /, 
+        pid: Optional[int] = None, 
+        page_size: int = 1150, 
+    ) -> Iterator[dict]:
+        if page_size <= 0:
+            page_size = 1150
+        payload = {
+            "file_id": self.get_id(id_or_path, pid), 
+            "offset": 0, 
+            "limit": page_size, 
+            "format": "json", 
+        }
+        while True:
+            data = check_response(self.client.fs_get_repeat(payload))["data"]
+            yield from data
+            if len(data) < page_size:
+                break
+            payload["offset"] += page_size # type: ignore
+
     def labels(
         self, 
         id_or_path: IDOrPathType = "", 
         /, 
         pid: Optional[int] = None, 
     ) -> list[dict]:
         return self.attr(id_or_path, pid)["labels"]
@@ -6926,25 +6961,34 @@
             if fid == 0:
                 return 0
             self.client.fs_score(fid, score)
             return score
 
     def search(
         self, 
-        search_value: str, 
         id_or_path: IDOrPathType = "", 
         /, 
         pid: Optional[int] = None, 
+        search_value: str = "", 
         page_size: int = 1_000, 
         offset: int = 0, 
         **kwargs, 
     ) -> Iterator[P115Path]:
         assert page_size > 0
+        attr = self.attr(id_or_path, pid)
+        if attr["is_directory"]:
+            if not search_value:
+                return
+            cid = attr["id"]
+        else:
+            if not search_value:
+                search_value = attr["sha1"]
+            cid = 0
         payload = {
-            "cid": self.get_id(id_or_path, pid), 
+            "cid": cid, 
             "search_value": search_value, 
             "limit": page_size, 
             "offset": offset, 
             **kwargs, 
         }
         def wrap(attr):
             attr = normalize_info(attr, fs=self, last_update=last_update)
@@ -8348,15 +8392,15 @@
         id_or_name: int | str, 
         /, 
     ) -> Iterator[P115Path]:
         if isinstance(id_or_name, int):
             id = id_or_name
         else:
             id = self[id_or_name]["id"]
-        return self.client.fs.search("", 0, file_label=id)
+        return self.client.fs.search(0, file_label=id)
 
     def list(
         self, 
         /, 
         offset: int = 0, 
         limit: int = 0, 
         keyword: str = "",
```

### Comparing `python_115-0.0.7.2/p115/cmd/iterdir.py` & `python_115-0.0.7.3/p115/cmd/iterdir.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 # coding: utf-8
 
 __author__ = "ChenyangGao <https://chenyanggao.github.io>"
 __all__: list[str] = []
 __doc__ = "115 文件夹信息遍历导出"
 
 KEYS = (
-    "id", "parent_id", "name", "path", "sha1", "pickcode", "is_directory", 
-    "size", "ctime", "mtime", "atime", "hidden", "violated", "play_long", 
-    "thumb", "star", "score", "labels", "description", 
+    "id", "parent_id", "name", "path", "relpath", "sha1", "pickcode", "is_directory", 
+    "size", "ctime", "mtime", "atime", "hidden", "violated", "play_long", "thumb", 
+    "star", "score", "labels", "description", 
 )
 
 if __name__ == "__main__":
     from argparse import ArgumentParser, RawTextHelpFormatter
 
     parser = ArgumentParser(description=__doc__, formatter_class=RawTextHelpFormatter)
 else:
@@ -51,17 +51,19 @@
 
     keys = args.keys or KEYS
     output_type = args.output_type
 
     path = args.path
     if path.isdecimal():
         fid = int(path)
+        attr = fs.attr(fid)
     else:
         attr = fs.attr(path)
         fid = attr["id"]
+    top_start = len(attr["path"]) + 1
 
     select = args.select
     if select:
         if select.startswith("lambda "):
             predicate = eval(select)
         else:
             predicate = eval("lambda path:" + select)
@@ -118,15 +120,46 @@
             speed = total / (cur_t - start_t)
             write(f"\r\x1b[K🗂️  {total} = 📂 {ndirs} + 📝 {nfiles} | 🕙 {format_time(cur_t-start_t)} | 🚀 {speed:.3f} it/s".encode())
         file = open(output_file, "w")
         path_it = iter(progress(path_it))
     else:
         file = stdout # type: ignore
 
-    records = ({k: p.get(k) if k != "description" else p.description for k in keys} for p in path_it)
+    from textwrap import dedent
+
+    dump_code = dedent(args.dump).strip()
+    if dump_code:
+        if args.dump_exec:
+            ns: dict = {}
+            exec(dump_code, ns)
+            dump = ns["dump"]
+        else:
+            code = compile(dump_code, "", "eval")
+            dump = lambda path: eval(code, {"path": path})
+        if output_file:
+            write = file.buffer.write
+        else:
+            write = file.buffer.raw.write # type: ignore
+        for path in path_it:
+            result = dump(path)
+            if not (result is None or isinstance(result, bytes)):
+                result = bytes(str(result), "utf-8")
+            if result:
+                write(result)
+        return
+
+    def get_key(path, key):
+        if key == "description":
+            return path.description
+        elif key == "relpath":
+            return path["path"][top_start:]
+        else:
+            return path.get(key)
+
+    records = ({k: get_key(p, k) for k in keys} for p in path_it)
 
     dumps: Callable[..., bytes]
     if output_type in ("log", "json"):
         try:
             from orjson import dumps
         except ImportError:
             odumps: Callable[..., str]
@@ -168,21 +201,27 @@
         file.close()
 
 
 parser.add_argument("path", nargs="?", default="0", help="文件夹路径或 id，默认值 0，即根目录")
 parser.add_argument("-c", "--cookie", help="115 登录 cookie，如果缺失，则从 115-cookie.txt 文件中获取，此文件可以在 当前工作目录、此脚本所在目录 或 用户根目录 下")
 parser.add_argument("-p", "--password", help="密码，用于进入隐藏模式，罗列隐藏文件")
 parser.add_argument("-k", "--keys", nargs="*", choices=KEYS, help=f"选择输出的 key，默认输出所有可选值")
+parser.add_argument("-d", "--dump", default="", help="""\
+(优先级高于 -k/--keys 和 -t/--output-type) 提供一段代码，每次调用，用于输出。
+如果结果 result 是
+    - None，跳过
+    - bytes，输出
+    - 其它，先调用 `bytes(str(result), 'utf-8')`，再输出""")
+parser.add_argument("-de", "--dump-exec", action="store_true", help="对 dump 代码进行 exec 解析（必须生成一个变量 dump，用于调用），否则用 eval 解析（会注入一个变量 path，类型是 p115.P115Path）")
 parser.add_argument("-s", "--select", help="提供一个表达式（会注入一个变量 path，类型是 p115.P115Path），用于对路径进行筛选")
-parser.add_argument("-t", "--output-type", choices=("log", "json", "csv"), default="log", help="""
+parser.add_argument("-t", "--output-type", choices=("log", "json", "csv"), default="log", help="""\
 输出类型，默认为 log
-- log   每行输出一条数据，每条数据输出为一个 json 的 object
-- json  输出一个 json 的 list，每条数据输出为一个 json 的 object
-- csv   输出一个 csv，第 1 行为表头，以后每行输出一条数据
-""")
+    - log   每行输出一条数据，每条数据输出为一个 json 的 object
+    - json  输出一个 json 的 list，每条数据输出为一个 json 的 object
+    - csv   输出一个 csv，第 1 行为表头，以后每行输出一条数据""")
 parser.add_argument("-o", "--output-file", help="保存到文件，此时命令行会输出进度条")
 parser.add_argument("-m", "--min-depth", default=0, type=int, help="最小深度，默认值 0，小于或等于 0 时不限")
 parser.add_argument("-M", "--max-depth", default=-1, type=int, help="最大深度，默认值 -1，小于 0 时不限")
 parser.add_argument("-dfs", "--depth-first", action="store_true", help="使用深度优先搜索，否则使用广度优先")
 parser.add_argument("-v", "--version", action="store_true", help="输出版本号")
 parser.set_defaults(func=main)
```

### Comparing `python_115-0.0.7.2/p115/cmd/qrcode.py` & `python_115-0.0.7.3/p115/cmd/qrcode.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.7.2/p115/tool/__init__.py` & `python_115-0.0.7.3/p115/tool/__init__.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.7.2/p115/util/_init_mimetypes.py` & `python_115-0.0.7.3/p115/util/_init_mimetypes.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.7.2/p115/util/cipher.py` & `python_115-0.0.7.3/p115/util/cipher.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.7.2/p115/util/concurrent.py` & `python_115-0.0.7.3/p115/util/concurrent.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.7.2/p115/util/download.py` & `python_115-0.0.7.3/p115/util/download.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.7.2/p115/util/file.py` & `python_115-0.0.7.3/p115/util/file.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.7.2/p115/util/hash.py` & `python_115-0.0.7.3/p115/util/hash.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.7.2/p115/util/ignore.py` & `python_115-0.0.7.3/p115/util/ignore.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.7.2/p115/util/iter.py` & `python_115-0.0.7.3/p115/util/iter.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.7.2/p115/util/path.py` & `python_115-0.0.7.3/p115/util/path.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.7.2/p115/util/property.py` & `python_115-0.0.7.3/p115/util/property.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.7.2/p115/util/response.py` & `python_115-0.0.7.3/p115/util/response.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.7.2/p115/util/retry.py` & `python_115-0.0.7.3/p115/util/retry.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.7.2/p115/util/text.py` & `python_115-0.0.7.3/p115/util/text.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.7.2/p115/util/urlopen.py` & `python_115-0.0.7.3/p115/util/urlopen.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.7.2/pyproject.toml` & `python_115-0.0.7.3/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "python-115"
-version = "0.0.7.2"
+version = "0.0.7.3"
 description = "Python wrapper for 115 webdisk."
 authors = ["ChenyangGao <wosiwujm@gmail.com>"]
 license = "MIT"
 readme = "readme.md"
 homepage = "https://github.com/ChenyangGao/web-mount-packs/tree/main/python-115-client"
 repository = "https://github.com/ChenyangGao/web-mount-packs/tree/main/python-115-client"
 keywords = ["nas", "115"]
```

### Comparing `python_115-0.0.7.2/readme.md` & `python_115-0.0.7.3/readme.md`

 * *Files identical despite different names*

### Comparing `python_115-0.0.7.2/PKG-INFO` & `python_115-0.0.7.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-115
-Version: 0.0.7.2
+Version: 0.0.7.3
 Summary: Python wrapper for 115 webdisk.
 Home-page: https://github.com/ChenyangGao/web-mount-packs/tree/main/python-115-client
 License: MIT
 Keywords: nas,115
 Author: ChenyangGao
 Author-email: wosiwujm@gmail.com
 Requires-Python: >=3.11,<4.0
```

