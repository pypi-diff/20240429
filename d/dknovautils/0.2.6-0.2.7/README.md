# Comparing `tmp/dknovautils-0.2.6.tar.gz` & `tmp/dknovautils-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dknovautils-0.2.6.tar", last modified: Thu Feb  1 13:26:43 2024, max compression
+gzip compressed data, was "dknovautils-0.2.7.tar", last modified: Mon Apr 29 03:20:09 2024, max compression
```

## Comparing `dknovautils-0.2.6.tar` & `dknovautils-0.2.7.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0 dknova    (1000) dknova    (1000)        0 2024-02-01 13:26:43.223645 dknovautils-0.2.6/
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)     1091 2023-05-19 02:33:35.000000 dknovautils-0.2.6/LICENSE
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)      910 2024-02-01 13:26:43.210637 dknovautils-0.2.6/PKG-INFO
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)      165 2024-01-30 05:58:19.000000 dknovautils-0.2.6/README.md
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)     2398 2024-02-01 13:26:36.000000 dknovautils-0.2.6/pyproject.toml
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)       38 2024-02-01 13:26:43.223645 dknovautils-0.2.6/setup.cfg
-drwxrwxrwx   0 dknova    (1000) dknova    (1000)        0 2024-02-01 13:26:43.177038 dknovautils-0.2.6/src/
-drwxrwxrwx   0 dknova    (1000) dknova    (1000)        0 2024-02-01 13:26:43.193725 dknovautils-0.2.6/src/dknovautils/
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)      326 2024-01-25 15:30:10.000000 dknovautils-0.2.6/src/dknovautils/__init__.py
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)      134 2024-01-25 15:30:06.000000 dknovautils-0.2.6/src/dknovautils/__main__.py
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)     2907 2024-02-01 04:42:06.000000 dknovautils-0.2.6/src/dknovautils/commons.py
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)     1229 2024-02-01 13:26:36.000000 dknovautils-0.2.6/src/dknovautils/dk_imports.py
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)     6828 2024-01-25 19:13:32.000000 dknovautils-0.2.6/src/dknovautils/dk_lang_etc_util.py
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)    16149 2024-02-01 13:26:36.000000 dknovautils-0.2.6/src/dknovautils/dkat.py
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)     2706 2024-01-26 10:06:48.000000 dknovautils-0.2.6/src/dknovautils/dkfiles.py
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)     1434 2024-01-25 19:12:29.000000 dknovautils-0.2.6/src/dknovautils/dkipy.py
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)     3634 2024-02-01 13:26:05.000000 dknovautils-0.2.6/src/dknovautils/dkprocess.py
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)      618 2024-01-25 09:56:51.000000 dknovautils-0.2.6/src/dknovautils/example.py
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)      282 2024-01-25 09:56:22.000000 dknovautils-0.2.6/src/dknovautils/myadd.py
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)      314 2024-01-25 15:05:17.000000 dknovautils-0.2.6/src/dknovautils/mysubtract.py
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)        0 2024-01-25 17:59:24.000000 dknovautils-0.2.6/src/dknovautils/py.typed
-drwxrwxrwx   0 dknova    (1000) dknova    (1000)        0 2024-02-01 13:26:43.210637 dknovautils-0.2.6/src/dknovautils.egg-info/
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)      910 2024-02-01 13:26:43.000000 dknovautils-0.2.6/src/dknovautils.egg-info/PKG-INFO
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)      677 2024-02-01 13:26:43.000000 dknovautils-0.2.6/src/dknovautils.egg-info/SOURCES.txt
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)        1 2024-02-01 13:26:43.000000 dknovautils-0.2.6/src/dknovautils.egg-info/dependency_links.txt
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)       43 2024-02-01 13:26:43.000000 dknovautils-0.2.6/src/dknovautils.egg-info/entry_points.txt
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)       14 2024-02-01 13:26:43.000000 dknovautils-0.2.6/src/dknovautils.egg-info/requires.txt
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)       12 2024-02-01 13:26:43.000000 dknovautils-0.2.6/src/dknovautils.egg-info/top_level.txt
-drwxrwxrwx   0 dknova    (1000) dknova    (1000)        0 2024-02-01 13:26:43.210637 dknovautils-0.2.6/tests/
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)      172 2024-01-26 10:01:40.000000 dknovautils-0.2.6/tests/test_b.py
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)      220 2024-01-26 10:01:52.000000 dknovautils-0.2.6/tests/test_c.py
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)     2331 2024-01-26 10:29:43.000000 dknovautils-0.2.6/tests/test_d.py
+drwxrwxrwx   0 dknova    (1000) dknova    (1000)        0 2024-04-29 03:20:09.719024 dknovautils-0.2.7/
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)     1091 2023-05-19 02:33:35.000000 dknovautils-0.2.7/LICENSE
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)      914 2024-04-29 03:20:09.718015 dknovautils-0.2.7/PKG-INFO
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)      169 2024-02-02 04:40:13.000000 dknovautils-0.2.7/README.md
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)     2398 2024-04-29 03:20:01.000000 dknovautils-0.2.7/pyproject.toml
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)       38 2024-04-29 03:20:09.719024 dknovautils-0.2.7/setup.cfg
+drwxrwxrwx   0 dknova    (1000) dknova    (1000)        0 2024-04-29 03:20:09.673016 dknovautils-0.2.7/src/
+drwxrwxrwx   0 dknova    (1000) dknova    (1000)        0 2024-04-29 03:20:09.699007 dknovautils-0.2.7/src/dknovautils/
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)      326 2024-01-25 15:30:10.000000 dknovautils-0.2.7/src/dknovautils/__init__.py
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)      134 2024-01-25 15:30:06.000000 dknovautils-0.2.7/src/dknovautils/__main__.py
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)     2907 2024-02-01 04:42:06.000000 dknovautils-0.2.7/src/dknovautils/commons.py
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)     1229 2024-04-29 03:20:01.000000 dknovautils-0.2.7/src/dknovautils/dk_imports.py
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)     6828 2024-01-25 19:13:32.000000 dknovautils-0.2.7/src/dknovautils/dk_lang_etc_util.py
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)    17331 2024-04-29 03:20:01.000000 dknovautils-0.2.7/src/dknovautils/dkat.py
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)     3332 2024-04-29 02:00:28.000000 dknovautils-0.2.7/src/dknovautils/dkfiles.py
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)     1447 2024-04-19 11:27:14.000000 dknovautils-0.2.7/src/dknovautils/dkipy.py
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)     4052 2024-04-29 02:59:04.000000 dknovautils-0.2.7/src/dknovautils/dkprocess.py
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)      618 2024-01-25 09:56:51.000000 dknovautils-0.2.7/src/dknovautils/example.py
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)      282 2024-01-25 09:56:22.000000 dknovautils-0.2.7/src/dknovautils/myadd.py
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)      314 2024-01-25 15:05:17.000000 dknovautils-0.2.7/src/dknovautils/mysubtract.py
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)        0 2024-01-25 17:59:24.000000 dknovautils-0.2.7/src/dknovautils/py.typed
+drwxrwxrwx   0 dknova    (1000) dknova    (1000)        0 2024-04-29 03:20:09.717018 dknovautils-0.2.7/src/dknovautils.egg-info/
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)      914 2024-04-29 03:20:09.000000 dknovautils-0.2.7/src/dknovautils.egg-info/PKG-INFO
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)      677 2024-04-29 03:20:09.000000 dknovautils-0.2.7/src/dknovautils.egg-info/SOURCES.txt
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)        1 2024-04-29 03:20:09.000000 dknovautils-0.2.7/src/dknovautils.egg-info/dependency_links.txt
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)       43 2024-04-29 03:20:09.000000 dknovautils-0.2.7/src/dknovautils.egg-info/entry_points.txt
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)       14 2024-04-29 03:20:09.000000 dknovautils-0.2.7/src/dknovautils.egg-info/requires.txt
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)       12 2024-04-29 03:20:09.000000 dknovautils-0.2.7/src/dknovautils.egg-info/top_level.txt
+drwxrwxrwx   0 dknova    (1000) dknova    (1000)        0 2024-04-29 03:20:09.715020 dknovautils-0.2.7/tests/
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)      172 2024-01-26 10:01:40.000000 dknovautils-0.2.7/tests/test_b.py
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)      220 2024-01-26 10:01:52.000000 dknovautils-0.2.7/tests/test_c.py
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)     3700 2024-04-29 03:16:44.000000 dknovautils-0.2.7/tests/test_d.py
```

### Comparing `dknovautils-0.2.6/LICENSE` & `dknovautils-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `dknovautils-0.2.6/PKG-INFO` & `dknovautils-0.2.7/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dknovautils
-Version: 0.2.6
+Version: 0.2.7
 Summary: A small example package
 Author-email: dknova <dikisite@outlook.com>, dknova2 <dikisite2@outlook.com>
 License: MIT License
 Project-URL: Homepage, https://example.com/xxx
 Project-URL: Documentation, https://readthedocs.org/xxx
 Project-URL: Repository, https://github.com/me/xxx.git
 Project-URL: Issues, https://github.com/me/xxx/issues
@@ -14,12 +14,12 @@
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: ipython
 
-#### some utilities frequently used by myself
+#### some utilities frequently used by the author
 
 The author doesn't suggest anyone else useing it. The api is not stable enough to be used as a public library.
```

### Comparing `dknovautils-0.2.6/pyproject.toml` & `dknovautils-0.2.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 # 之所以改成setuptools build 是因为要配置 py.typed参数 而如果用hatch工具不知道如何配置
 [build-system]
 requires = ["setuptools >= 61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dknovautils"
-version = '0.2.6'
+version = '0.2.7'
 dependencies = [
     "numpy",
     "ipython"
 ]
 authors = [
   { name="dknova", email="dikisite@outlook.com" },
   { name="dknova2", email="dikisite2@outlook.com" },
```

### Comparing `dknovautils-0.2.6/src/dknovautils/commons.py` & `dknovautils-0.2.7/src/dknovautils/commons.py`

 * *Files identical despite different names*

### Comparing `dknovautils-0.2.6/src/dknovautils/dk_imports.py` & `dknovautils-0.2.7/src/dknovautils/dk_imports.py`

 * *Files identical despite different names*

### Comparing `dknovautils-0.2.6/src/dknovautils/dk_lang_etc_util.py` & `dknovautils-0.2.7/src/dknovautils/dk_lang_etc_util.py`

 * *Files identical despite different names*

### Comparing `dknovautils-0.2.6/src/dknovautils/dkat.py` & `dknovautils-0.2.7/src/dknovautils/dkat.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,29 @@
 from __future__ import annotations
 
 
 import http.server
 from logging import Logger, LoggerAdapter
 import socketserver
+from typing import TypeVar
 from typing_extensions import override
 
+
 import dknovautils
 
 # from dknovautils.dk_imports import *
 from dknovautils.commons import *
 
 
-DkAppVer = '0.2.6'
+DkAppVer = '0.2.7'
 
 _unknown_err = "_unknown_err4035"
 
+T = TypeVar("T")
+
 
 class staticproperty(property):
     """
     https://stackoverflow.com/questions/1697501/staticmethod-with-property
 
     """
 
@@ -72,15 +76,17 @@
         return r
 
     @classmethod
     def _create_my_logger_adapter(cls) -> MyLoggerAdapter:
         class _MyLoggerAdapter(MyLoggerAdapter):
             # todo 这个 args kwargs 如何标注类型?
             @override
-            def log(self, level: int, msg: object, *args, **kwargs ) -> None:  # type:ignore
+            def log(
+                self, level: int, msg: object, *args, **kwargs  # type:ignore
+            ) -> None:  # type:ignore
                 if level == LLevel.Warn.value:
                     AT._AstWarnCnt_ += 1
                 elif level >= LLevel.Error.value:
                     AT._AstErrorCnt_ += 1
                 else:
                     pass
 
@@ -112,15 +118,15 @@
         beepError: bool = False,
         beepWarn: bool = False,
     ) -> Callable[[object, LLevel], None]:
         """
         创建一个logger 作为系统的缺省logger
         """
 
-        def mloggerFun(obj: object, llevel: LLevel) -> None:
+        def m_logger_fun(obj: object, llevel: LLevel) -> None:
             assert isinstance(llevel, LLevel)
             _logger = cls.get_logger()
 
             if False:
                 pass
             elif llevel == LLevel.Trace:
                 # 也用debug级别。只是在prod模式下可以关闭。
@@ -137,18 +143,19 @@
                 _logger.error(obj)
                 if beepError:
                     AT.beep_error_buffered()
             else:
                 assert False, f"bad {llevel}"
 
         if initInnerLoggerFun:
-            cls._logger_adapter = None  # force refetch logger
-            AT._inner_logger_fun = mloggerFun
+            cls._logger_adapter = None  # force recreate
+            cls.get_logger()
+            AT._inner_logger_fun = m_logger_fun
 
-        return mloggerFun
+        return m_logger_fun
 
     _LOG_FORMAT_100 = "%(asctime)s - %(levelname)s - %(message)s"
     _DATE_FORMAT_100 = "%m/%d/%Y %H:%M:%S %p"
     # _DATE_FORMAT_iso_simple = "%m/%d/%Y %H:%M:%S %p"
 
     STRFMT_ISO_COMPACT_SIMPLE = "%Y%m%dT%H%M%S"
     STRFMT_ISO_COMPACT_ALL_A = "%Y%m%dT%H%M%SS%fZ%Z"
@@ -423,15 +430,15 @@
 
         d date
         s seconds
         ms millis
         a all
 
         """
-        assert precise in ["d", "s", "ms", "a"], "err5554 bad precise"
+        assert precise in ("d", "s", "ms", "a"), "err5554 bad precise"
 
         if dt is not None and isinstance(dt, int):
             dt = datetime.fromtimestamp(dt / 1000, tz=None)
         elif dt is None:
             dt = datetime.now()
         else:
             pass
@@ -534,46 +541,79 @@
                 if not data:
                     break
                 m.update(data)  # 更新md5对象
 
         return m.hexdigest().lower()  # 返回md5对象
 
     @classmethod
-    def bindport_httpserver(cls, *, port: int, daemon: bool = False) -> bool:
+    def list_unique(cls, ls: List[T]) -> List[T]:
+        d = {ln: None for ln in ls}
+        lns = list(d.keys())
+        return lns
+
+    @classmethod
+    def bindport_httpserver(
+        cls, *, port: int, daemon: bool = False
+    ) -> socketserver.TCPServer | None:
         """
-        如果绑定成功 将启动一个线程 长期占用该端口 并返回 True
-        否则返回 False
+        如果绑定端口成功 将启动一个线程 持续占用该端口 并返回 TcpServer
+        否则返回 None
 
         """
         AT.assert_(port > 0, "err10591 port error")
         PORT = port
         Handler = http.server.SimpleHTTPRequestHandler
+        server = None
+        startOk = False
 
         try:
-            startOk = True
 
             def tf() -> None:
+                nonlocal server
                 nonlocal startOk
                 try:
                     with socketserver.TCPServer(("", PORT), Handler) as httpd:
                         iprint_debug(f"serving at port {port}")
+                        server = httpd
+                        startOk = True
                         httpd.serve_forever()
                 except:
                     startOk = False
 
             thread = threading.Thread(target=tf, args=(), daemon=daemon)
             thread.start()
 
-            time.sleep(1.0)
+            time.sleep(0.5)
             iprint_debug(f"bind tcp port ok. {port} {startOk}")
-            return startOk
+            return server
 
         except Exception as e:
-            iprint_debug(f"some err here: {e}")
-            return False
+            iprint_debug(f"some err occured: {e}")
+            return None
+
+    @classmethod
+    def bindport_httpserver_cb(
+        cls, *, port: int, cb: Callable[[], None]
+    ) -> socketserver.TCPServer | None:
+        """
+        如果绑定端口成功 将启动一个daemon线程 持续占用该端口 然后执行cb回调函数. 返回 TCPServer
+        如果绑定端口不成功 将直接 返回 None
+
+        """
+        AT.assert_(port > 0 and cb, "err27617")
+        server = cls.bindport_httpserver(port=port, daemon=True)
+        if server:
+            try:
+                cb()
+            except Exception as e:
+                iprint_warn(f"error78836 {e}")
+            finally:
+                return server
+        else:
+            return None
 
     # end
     VERSION = DkAppVer
 
 
 class DkAstException(Exception):
     pass
```

### Comparing `dknovautils-0.2.6/src/dknovautils/dkfiles.py` & `dknovautils-0.2.7/src/dknovautils/dkfiles.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,41 +1,65 @@
 from __future__ import annotations
 
 from dknovautils.commons import *
 
+import pathlib
+
+
 _debug = False
 
 
 class DkFile(object):
     def __init__(self, pathstr: str) -> None:
         self.pathstr = str(pathstr)
 
         self.path = Path(pathstr)
 
+    def __key(self) -> Any:
+        return self.path
+
+    def __hash__(self) -> int:
+        return hash(self.__key())
+
+    def __eq__(self, other:Any) -> Any:
+        if isinstance(other, DkFile):
+            return self.__key() == other.__key()
+        return NotImplemented
+
     @property
     def basename(self) -> str:
         return os.path.basename(self.path)
 
     @property
     def filesize(self) -> int:
         return getsize(self.path)
 
     @property
     def dirname(self) -> str:
         return os.path.dirname(self.path)
 
+    @property
+    def extension(self) -> str:
+        """包括点号 比如 .txt 如果没有扩展名 则返回空串 """
+        # function to return the file extension
+        file_extension = self.path.suffix
+        return file_extension
+
     def exists(self) -> bool:
         return self.path.exists()
 
     def is_file(self) -> bool:
         return self.path.is_file()
 
     def is_dir(self) -> bool:
         return self.path.is_dir()
 
+    def __repr__(self) -> str:
+        return self.__str__()
+
     def __str__(self) -> str:
         return str(self.path)
 
     @staticmethod
     def clear_dir(folder: str) -> None:
         """
```

### Comparing `dknovautils-0.2.6/src/dknovautils/dkipy.py` & `dknovautils-0.2.7/src/dknovautils/dkipy.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,9 @@
 from __future__ import annotations
 
-# from dknovautils.dk_imports import *
-
-# from typing import Any
 
 # 导入module 而不是导入函数或者类 可以避免循环import的问题
 from dknovautils import commons
 from dknovautils.commons import *
 
 
 class DkIpyUtils(object):
@@ -19,14 +16,15 @@
     def mfc(cmd: str, logcmd: bool = True) -> None:
         DkIpyUtils.mfr(cmd, logcmd)
 
     _cmd_id = 1000
 
     @staticmethod
     def mfr(cmd: str, logcmd: bool = True) -> Any:
+        # 这样局部import 只有执行这个函数的时候 才依赖ipython
         from IPython.core.getipython import get_ipython  # type ignore[import-untyped]
 
         assert isinstance(cmd, str) and len(cmd) > 0, "err3581"
         DkIpyUtils._cmd_id += 1
         if logcmd:
             commons.iprint_info(f"run cmd begin {DkIpyUtils._cmd_id}: {cmd}")
```

### Comparing `dknovautils-0.2.6/src/dknovautils/dkprocess.py` & `dknovautils-0.2.7/src/dknovautils/dkprocess.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,51 +1,56 @@
 from __future__ import annotations
 
-# import subprocess
-# import sys
-# from typing import List, Tuple
-# from dknovautils.dk_imports import *
 
 # 导入module避免某些循环import的问题
 from dknovautils import commons, iprint_debug, iprint_warn, AT  # type:ignore
 from dknovautils.commons import *
 
 
 class DKProcessUtil(object):
     _cmdid = 1000
 
+    _retcode_default: int = -999
+
     # 这个例子说明 call() 函数具有不可替代的价值。
     @staticmethod
-    def run_simple_a(cmd: str, _debug: bool = False) -> None:
+    def run_simple_a(cmd: str, _debug: bool = False) -> int:
         cmdid = DKProcessUtil._cmdid
         DKProcessUtil._cmdid += 1
 
         if _debug:
-            iprint_debug(f"run_simple_a {cmdid} " + cmd[:300])
+            iprint_debug(f"run_simple_a {cmdid} {cmd[:300]}")
+
+        retcode: int = DKProcessUtil._retcode_default
 
         try:
             retcode = subprocess.call(cmd, shell=True)
             if retcode < 0 and _debug:
-                iprint_debug(
-                    "Child was terminated by signal", -retcode, file=sys.stderr
-                )
+                iprint_debug(f"Child was terminated by signal {retcode}")
             elif _debug:
-                iprint_debug("Child returned", retcode, file=sys.stderr)
+                iprint_debug(f"Child returned {retcode}")
         except OSError as e:
-            iprint_warn(f"run_simple_a {cmdid} Execution failed:", e, file=sys.stderr)
+            iprint_warn(f"run_simple_a {cmdid} Execution failed: {e}")
+
+        return retcode
 
     @staticmethod
     def run_simple_b(
         cmd: str,
         *,
         splitLines: bool = False,
         throwOnErrReturnCode: bool = False,
+        strip: bool = True,
         _debug: bool = False,
+        encoding: Any = None,
+        errors:Any=None,
     ) -> Tuple[int, str, str]:
-        """ """
+        """ 
+        
+        """
         # Tuple[int, str|List,str|List]
         cmdid = DKProcessUtil._cmdid
         DKProcessUtil._cmdid += 1
 
         AT.assert_(not splitLines, "err51042 no splitlines")
 
         if _debug:
@@ -55,14 +60,16 @@
         # 运行中，会缓存结果，直到执行完成才会输出。
         sp = subprocess.Popen(
             cmd,
             shell=True,
             universal_newlines=True,
             stdout=subprocess.PIPE,
             stderr=subprocess.PIPE,
+            encoding=encoding,
+            errors=errors,
         )
 
         # Store the return code in rc variable
         # 这个rc值如何获取？如果打开这一行，将在某些情况下产生死锁问题。
         # 来自文档中的说明: This will deadlock when using stdout=PIPE or stderr=PIPE and the child process generates enough output to a pipe such that it blocks waiting for the OS pipe buffer to accept more data. Use Popen.communicate() when using pipes to avoid that.
         # rc = sp.wait()
 
@@ -82,26 +89,36 @@
             iprint_debug(f"run_simple_b end {cmdid}")
 
         if out is None:
             out = ""
         if err is None:
             err = ""
 
+        if strip:
+            out = out.strip()
+            err = err.strip()
+
         if throwOnErrReturnCode and (rc != 0):
-            msg = f"cmd {cmdid} run error. cmd: {cmd} err: {rc} {err}"
+            msg = f"cmd {cmdid} run error. err: {rc} {err}"
             raise Exception(msg)
 
-        return (rc, out, err)
+        """
+        
+        这个函数发现的问题之一 是在wsl中执行robocopy等win命令时 会输出非unicode编码的字符 从而导致out解码出现错误.
+        有时候似乎加上encoding也不行. 比如 encoding='utf-16'也是不行的
+        
+        关于encoding errors 参考如下文档
+        https://docs.python.org/3/howto/unicode.html
+        https://docs.python.org/3/library/io.html#io.TextIOWrapper
+        
+        
+        
+        """
 
-        # if False and splitLines:
-        #     # out = out.splitlines()
-        #     # err = err.splitlines()
-        #     return (rc, out.splitlines(), err.splitlines())
-        # else:
-        #     return (rc, out, err)
+        return (rc, out, err)
 
 
 run_simple_a = DKProcessUtil.run_simple_a
 run_simple_b = DKProcessUtil.run_simple_b
 
 
 """
```

### Comparing `dknovautils-0.2.6/src/dknovautils/example.py` & `dknovautils-0.2.7/src/dknovautils/example.py`

 * *Files identical despite different names*

### Comparing `dknovautils-0.2.6/src/dknovautils.egg-info/PKG-INFO` & `dknovautils-0.2.7/src/dknovautils.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dknovautils
-Version: 0.2.6
+Version: 0.2.7
 Summary: A small example package
 Author-email: dknova <dikisite@outlook.com>, dknova2 <dikisite2@outlook.com>
 License: MIT License
 Project-URL: Homepage, https://example.com/xxx
 Project-URL: Documentation, https://readthedocs.org/xxx
 Project-URL: Repository, https://github.com/me/xxx.git
 Project-URL: Issues, https://github.com/me/xxx/issues
@@ -14,12 +14,12 @@
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: ipython
 
-#### some utilities frequently used by myself
+#### some utilities frequently used by the author
 
 The author doesn't suggest anyone else useing it. The api is not stable enough to be used as a public library.
```

### Comparing `dknovautils-0.2.6/src/dknovautils.egg-info/SOURCES.txt` & `dknovautils-0.2.7/src/dknovautils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

