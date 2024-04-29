# Comparing `tmp/userspacefs-3.0.0.tar.gz` & `tmp/userspacefs-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "userspacefs-3.0.0.tar", last modified: Fri Jan  5 19:05:36 2024, max compression
+gzip compressed data, was "userspacefs-3.1.0.tar", last modified: Mon Apr 29 16:19:29 2024, max compression
```

## Comparing `userspacefs-3.0.0.tar` & `userspacefs-3.1.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 rian      (1000) rian      (1000)        0 2024-01-05 19:05:36.913059 userspacefs-3.0.0/
--rw-r--r--   0 rian      (1000) rian      (1000)    35142 2018-10-04 19:49:20.000000 userspacefs-3.0.0/LICENSE
--rw-r--r--   0 rian      (1000) rian      (1000)       16 2020-12-22 18:55:33.000000 userspacefs-3.0.0/MANIFEST.in
--rw-r--r--   0 rian      (1000) rian      (1000)      982 2024-01-05 19:05:36.913059 userspacefs-3.0.0/PKG-INFO
--rw-r--r--   0 rian      (1000) rian      (1000)      522 2024-01-05 01:14:55.000000 userspacefs-3.0.0/README.md
--rw-r--r--   0 rian      (1000) rian      (1000)       73 2024-01-05 19:05:36.913059 userspacefs-3.0.0/setup.cfg
--rw-r--r--   0 rian      (1000) rian      (1000)     1549 2024-01-05 18:54:10.000000 userspacefs-3.0.0/setup.py
-drwxr-xr-x   0 rian      (1000) rian      (1000)        0 2024-01-05 19:05:36.913059 userspacefs-3.0.0/userspacefs/
--rw-r--r--   0 rian      (1000) rian      (1000)    26310 2024-01-05 18:50:45.000000 userspacefs-3.0.0/userspacefs/__init__.py
--rw-r--r--   0 rian      (1000) rian      (1000)     6510 2023-12-28 19:43:40.000000 userspacefs-3.0.0/userspacefs/abc.py
--rw-r--r--   0 rian      (1000) rian      (1000)     9932 2023-12-26 13:51:30.000000 userspacefs-3.0.0/userspacefs/fuse_adapter.py
--rw-r--r--   0 rian      (1000) rian      (1000)    51008 2023-12-26 01:47:45.000000 userspacefs-3.0.0/userspacefs/fusepy.py
--rw-r--r--   0 rian      (1000) rian      (1000)     3810 2023-12-26 13:51:30.000000 userspacefs-3.0.0/userspacefs/macos_path_conversion.py
--rw-r--r--   0 rian      (1000) rian      (1000)    20355 2023-12-30 21:24:07.000000 userspacefs-3.0.0/userspacefs/memoryfs.py
--rw-r--r--   0 rian      (1000) rian      (1000)     3477 2023-12-21 20:00:35.000000 userspacefs-3.0.0/userspacefs/path_common.py
--rw-r--r--   0 rian      (1000) rian      (1000)        0 2023-11-12 06:49:30.000000 userspacefs-3.0.0/userspacefs/py.typed
--rw-r--r--   0 rian      (1000) rian      (1000)   152659 2023-12-26 14:26:11.000000 userspacefs-3.0.0/userspacefs/smbserver.py
--rw-r--r--   0 rian      (1000) rian      (1000)     3387 2023-12-26 13:51:30.000000 userspacefs-3.0.0/userspacefs/stdlibfs.py
--rw-r--r--   0 rian      (1000) rian      (1000)    13547 2024-01-05 01:14:55.000000 userspacefs-3.0.0/userspacefs/util_dumpster.py
--rw-r--r--   0 rian      (1000) rian      (1000)    51898 2023-12-30 21:24:07.000000 userspacefs-3.0.0/userspacefs/webdavserver.py
-drwxr-xr-x   0 rian      (1000) rian      (1000)        0 2024-01-05 19:05:36.913059 userspacefs-3.0.0/userspacefs.egg-info/
--rw-r--r--   0 rian      (1000) rian      (1000)      982 2024-01-05 19:05:36.000000 userspacefs-3.0.0/userspacefs.egg-info/PKG-INFO
--rw-r--r--   0 rian      (1000) rian      (1000)      530 2024-01-05 19:05:36.000000 userspacefs-3.0.0/userspacefs.egg-info/SOURCES.txt
--rw-r--r--   0 rian      (1000) rian      (1000)        1 2024-01-05 19:05:36.000000 userspacefs-3.0.0/userspacefs.egg-info/dependency_links.txt
--rw-r--r--   0 rian      (1000) rian      (1000)       82 2024-01-05 19:05:36.000000 userspacefs-3.0.0/userspacefs.egg-info/requires.txt
--rw-r--r--   0 rian      (1000) rian      (1000)       12 2024-01-05 19:05:36.000000 userspacefs-3.0.0/userspacefs.egg-info/top_level.txt
+drwxr-xr-x   0 rian      (1000) rian      (1000)        0 2024-04-29 16:19:29.538954 userspacefs-3.1.0/
+-rw-r--r--   0 rian      (1000) rian      (1000)    35142 2018-10-04 19:49:20.000000 userspacefs-3.1.0/LICENSE
+-rw-r--r--   0 rian      (1000) rian      (1000)       16 2020-12-22 18:55:33.000000 userspacefs-3.1.0/MANIFEST.in
+-rw-r--r--   0 rian      (1000) rian      (1000)      982 2024-04-29 16:19:29.538954 userspacefs-3.1.0/PKG-INFO
+-rw-r--r--   0 rian      (1000) rian      (1000)      522 2024-01-05 01:14:55.000000 userspacefs-3.1.0/README.md
+-rw-r--r--   0 rian      (1000) rian      (1000)       73 2024-04-29 16:19:29.538954 userspacefs-3.1.0/setup.cfg
+-rw-r--r--   0 rian      (1000) rian      (1000)     1549 2024-04-29 16:19:15.000000 userspacefs-3.1.0/setup.py
+drwxr-xr-x   0 rian      (1000) rian      (1000)        0 2024-04-29 16:19:29.538954 userspacefs-3.1.0/userspacefs/
+-rw-r--r--   0 rian      (1000) rian      (1000)    26813 2024-01-06 23:08:31.000000 userspacefs-3.1.0/userspacefs/__init__.py
+-rw-r--r--   0 rian      (1000) rian      (1000)     7064 2024-01-10 22:26:57.000000 userspacefs-3.1.0/userspacefs/abc.py
+-rw-r--r--   0 rian      (1000) rian      (1000)    10550 2024-01-10 23:11:45.000000 userspacefs-3.1.0/userspacefs/fuse_adapter.py
+-rw-r--r--   0 rian      (1000) rian      (1000)    51008 2024-01-19 20:55:58.000000 userspacefs-3.1.0/userspacefs/fusepy.py
+-rw-r--r--   0 rian      (1000) rian      (1000)     3810 2023-12-26 13:51:30.000000 userspacefs-3.1.0/userspacefs/macos_path_conversion.py
+-rw-r--r--   0 rian      (1000) rian      (1000)    20355 2023-12-30 21:24:07.000000 userspacefs-3.1.0/userspacefs/memoryfs.py
+-rw-r--r--   0 rian      (1000) rian      (1000)     3729 2024-01-10 22:42:18.000000 userspacefs-3.1.0/userspacefs/path_common.py
+-rw-r--r--   0 rian      (1000) rian      (1000)        0 2023-11-12 06:49:30.000000 userspacefs-3.1.0/userspacefs/py.typed
+-rw-r--r--   0 rian      (1000) rian      (1000)   153197 2024-01-10 22:44:33.000000 userspacefs-3.1.0/userspacefs/smbserver.py
+-rw-r--r--   0 rian      (1000) rian      (1000)     4150 2024-01-10 23:13:25.000000 userspacefs-3.1.0/userspacefs/stdlibfs.py
+-rw-r--r--   0 rian      (1000) rian      (1000)    13909 2024-01-08 01:51:34.000000 userspacefs-3.1.0/userspacefs/util_dumpster.py
+-rw-r--r--   0 rian      (1000) rian      (1000)    52348 2024-01-10 22:43:31.000000 userspacefs-3.1.0/userspacefs/webdavserver.py
+drwxr-xr-x   0 rian      (1000) rian      (1000)        0 2024-04-29 16:19:29.538954 userspacefs-3.1.0/userspacefs.egg-info/
+-rw-r--r--   0 rian      (1000) rian      (1000)      982 2024-04-29 16:19:29.000000 userspacefs-3.1.0/userspacefs.egg-info/PKG-INFO
+-rw-r--r--   0 rian      (1000) rian      (1000)      530 2024-04-29 16:19:29.000000 userspacefs-3.1.0/userspacefs.egg-info/SOURCES.txt
+-rw-r--r--   0 rian      (1000) rian      (1000)        1 2024-04-29 16:19:29.000000 userspacefs-3.1.0/userspacefs.egg-info/dependency_links.txt
+-rw-r--r--   0 rian      (1000) rian      (1000)       82 2024-04-29 16:19:29.000000 userspacefs-3.1.0/userspacefs.egg-info/requires.txt
+-rw-r--r--   0 rian      (1000) rian      (1000)       12 2024-04-29 16:19:29.000000 userspacefs-3.1.0/userspacefs.egg-info/top_level.txt
```

### Comparing `userspacefs-3.0.0/LICENSE` & `userspacefs-3.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `userspacefs-3.0.0/PKG-INFO` & `userspacefs-3.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: userspacefs
-Version: 3.0.0
+Version: 3.1.0
 Summary: Cross-platform user-space file systems for Python
 Home-page: https://thelig.ht/code/userspacefs
 Author: Rian Hunter
 Author-email: rian@alum.mit.edu
 License: GPL3
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3
```

### Comparing `userspacefs-3.0.0/README.md` & `userspacefs-3.1.0/README.md`

 * *Files identical despite different names*

### Comparing `userspacefs-3.0.0/setup.py` & `userspacefs-3.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 from setuptools import setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="userspacefs",
-    version='3.0.0',
+    version='3.1.0',
     author="Rian Hunter",
     author_email="rian@alum.mit.edu",
     description="Cross-platform user-space file systems for Python",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://thelig.ht/code/userspacefs',
     license="GPL3",
```

### Comparing `userspacefs-3.0.0/userspacefs/__init__.py` & `userspacefs-3.1.0/userspacefs/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -230,41 +230,42 @@
             webdav_url += ":%d" % (port,)
         webdav_url += path_root
         return webdav_url
     def mount(address: typing.Tuple[str, int], mount_point: str) -> None:
         # NB: this only works for Windows
         if sys.platform != 'win32':
             raise Exception("this platform not supported")
+        else:
+            drive_letter = mount_point[0]
 
-        drive_letter = mount_point[0]
-
-        webdav_url = create_url(address)
+            webdav_url = create_url(address)
 
-        log.debug("Mounting: %r", webdav_url)
+            log.debug("Mounting: %r", webdav_url)
 
-        tried = False
-        while True:
-            ret = subprocess.call(["net", "use", '%s:' % (drive_letter,),
-                                   "%s" % (webdav_url,),
-                                   "/persistent:no"],
-                                  creationflags=subprocess.CREATE_NO_WINDOW)
-            if not ret:
-                break
-            if not tried:
-                import win32com.shell.shell as shell
-                res = shell.ShellExecuteEx(
-                    lpVerb='runas',
-                    lpFile="%s\\System32\\sc" % (os.environ['SystemRoot'],),
-                    lpParameters="config WebClient start=auto",
-                )
-                if res:
-                    tried = True
-                    time.sleep(1)
-                    continue
-            raise Exception("failed mount! %d" % (ret,))
+            tried = False
+            while True:
+                ret = subprocess.call(["net", "use", '%s:' % (drive_letter,),
+                                       "%s" % (webdav_url,),
+                                       "/persistent:no"],
+                                      creationflags=subprocess.CREATE_NO_WINDOW)
+                if not ret:
+                    break
+                if not tried:
+                    import win32com.shell.shell as shell
+
+                    res = shell.ShellExecuteEx(
+                        lpVerb='runas',
+                        lpFile="%s\\System32\\sc" % (os.environ['SystemRoot'],),
+                        lpParameters="config WebClient start=auto",
+                    )
+                    if res:
+                        tried = True
+                        time.sleep(1)
+                        continue
+                raise Exception("failed mount! %d" % (ret,))
     def unmount(mount_point: str) -> None:
         # NB: this only works for Windows
         if sys.platform != 'win32':
             raise Exception("this platform not supported")
 
         drive_letter = mount_point[0]
 
@@ -601,15 +602,15 @@
         for kv in values.split(","):
             ret = kv.split("=", 1)
             if len(ret) == 2:
                 ns.o[ret[0]] = ret[1]
             else:
                 ns.o[ret[0]] = True
 
-def _add_simple_cli_arguments(parser: argparse.ArgumentParser) -> None:
+def add_simple_cli_arguments(parser: argparse.ArgumentParser) -> None:
     def ensure_listen_address(string: str) -> typing.Tuple[str, int]:
         try:
             (host, port_s) = string.split(":", 1)
         except ValueError:
             host = string
             port = 0
         else:
@@ -632,44 +633,55 @@
     parser.add_argument("-l", "--listen-address",
                         type=ensure_listen_address,
                         help="address that the filesystem server should listen on, append colon to specify port")
     parser.add_argument("-o", metavar='opt,[opt...]', action=_FUSEOption,
                         help="FUSE options, e.g. -o uid=1000,allow_other")
     parser.add_argument("-n", "--no-mount", action="store_true",
                         help="export filesystem via network server but don't mount it")
-    parser.add_argument("mount_point", nargs='?')
+
+def check_simple_args_result(
+        parser: argparse.ArgumentParser,
+        args : argparse.Namespace,
+) -> None:
+    if args.no_mount and not args.smb and not args.webdav:
+        parser.error("either --smb or --webdav must be specified when --no-mount is specified")
+
+def simple_main_with_args(
+        mount_point: typing.Optional[str],
+        display_name: str,
+        create_fs_params: typing.Tuple[str, typing.Mapping[str, typing.Any]],
+        args: argparse.Namespace,
+        **kw: typing.Any,
+) -> int:
+    return simple_main(mount_point, display_name, create_fs_params,
+                       foreground=args.foreground,
+                       smb_only=args.smb,
+                       webdav_only=args.webdav,
+                       no_mount=args.no_mount,
+                       listen_address=args.listen_address,
+                       fuse_options=args.o, **kw)
 
 def simple_main_from_argv(display_name: str,
                           create_fs_params: typing.Tuple[str, typing.Mapping[str, typing.Any]],
                           argv: typing.Optional[typing.Sequence[str]] = None) -> int:
     if argv is None:
         argv = sys.argv
 
     parser = argparse.ArgumentParser()
-    _add_simple_cli_arguments(parser)
+    add_simple_cli_arguments(parser)
     parser.add_argument("-v", "--verbose", action="count", default=0,
                         help="show log messages, use twice for maximum verbosity")
+    parser.add_argument("mount_point", nargs='?')
     args = parser.parse_args(argv[1:])
 
     level = [logging.WARNING, logging.INFO, logging.DEBUG][min(2, args.verbose)]
     logging.basicConfig(level=level)
 
     if args.mount_point is None and not args.no_mount:
-        print("error: the 'mount_point' argument is required unless --no-mount is specified",
-              file=sys.stderr)
-        return -1
+        parser.error("the 'mount_point' argument is required unless --no-mount is specified")
 
-    if args.no_mount and not args.smb and not args.webdav:
-        print("error: either --smb or --webdav must be specified when --no-mount is specified",
-              file=sys.stderr)
-        return -1
+    check_simple_args_result(parser, args)
 
-    return simple_main(args.mount_point, display_name, create_fs_params,
-                       foreground=args.foreground,
-                       smb_only=args.smb,
-                       webdav_only=args.webdav,
-                       no_mount=args.no_mount,
-                       listen_address=args.listen_address,
-                       fuse_options=args.o)
+    return simple_main_with_args(args.mount_point, display_name, create_fs_params, args)
 
 if __name__ == "__main__":
     sys.exit(main(sys.argv))
```

### Comparing `userspacefs-3.0.0/userspacefs/abc.py` & `userspacefs-3.1.0/userspacefs/abc.py`

 * *Files 18% similar despite different names*

```diff
@@ -138,14 +138,24 @@
         raise NotImplementedError()
 
     @property
     @abstractmethod
     def parent(self) -> typing.Self:
         raise NotImplementedError()
 
+    def with_name(self, name: str) -> typing.Self:
+        # NB: with_name() usually throws if the name contains a path
+        #     separator element, so this default method is not
+        #     strictly correct. It's OK in this context because
+        #     user-defined file systems usually don't have any concept
+        #     of a path separator or even a path-string. In a future
+        #     version this will be made abstract. not doing it now to
+        #     avoid a pointless major version change.
+        return self.parent.joinpath(name)
+
 # mimics os.statvfs() result
 class StatVFS(typing.Protocol):
     @property
     @abstractmethod
     def f_bavail(self) -> int:
         raise NotImplementedError()
```

### Comparing `userspacefs-3.0.0/userspacefs/fuse_adapter.py` & `userspacefs-3.1.0/userspacefs/fuse_adapter.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,17 +25,18 @@
 import threading
 import typing
 import stat
 import sys
 
 from collections.abc import Callable
 
-from userspacefs.abc import FileSystem, Path, File, Stat, Directory
+from userspacefs.abc import FileSystem, Path, File, Stat, Directory, DirEntry
 from userspacefs.fusepy import FUSE, fuse_file_info, Operations
 from userspacefs.util_dumpster import datetime_from_ts
+from userspacefs.path_common import join_name
 
 log = logging.getLogger(__name__)
 
 def check_mode(mode: int) -> None:
     if ((stat.S_IFCHR | stat.S_IFBLK | stat.S_IFIFO | stat.S_IFLNK | stat.S_IFSOCK) & mode) == (stat.S_IFCHR | stat.S_IFBLK | stat.S_IFIFO | stat.S_IFLNK | stat.S_IFSOCK):
         raise OSError(errno.EPERM, os.strerror(errno.EPERM))
 
@@ -78,15 +79,15 @@
             return self._fh_to_dir.pop(fh)
 
     def _conv_path(self, path: str) -> Path:
         assert self._fs is not None
         toret = self._fs.create_path()
         if path == '/':
             return toret
-        return toret.joinpath(*path[1:].split('/'))
+        return join_name(toret, *path[1:].split('/'))
 
     def _fs_stat_to_fuse_attrs(self, st: Stat) -> typing.Dict[str, typing.Any]:
         toret = {}
 
         toret['st_birthtime'] = getattr(st, "st_birthtime", 0)
         toret['st_mtime'] = getattr(st, "st_mtime", toret['st_birthtime'])
         toret['st_ctime'] = getattr(st, "st_ctime", toret['st_mtime'])
@@ -193,15 +194,29 @@
     def opendir(self, path: str) -> int:
         assert self._fs is not None
         return self._save_dir(self._fs.open_directory(self._conv_path(path)))
 
     def readdir(self, path: typing.Optional[str], fh: int) -> typing.List[str | typing.Tuple[str, typing.Dict[str, typing.Any], int]]:
         # TODO: pyfuse doesn't expose a better interface for large directories
         f = self._fh_to_dir[fh]
-        return list(itertools.chain(['.', '..'], map(lambda x: (x.name, self._fs_stat_to_fuse_attrs(x.stat()), 0), f)))
+
+        def transform_entry(x: DirEntry) -> typing.Tuple[str, typing.Dict[str, typing.Any], int] | str:
+            try:
+                st = x.stat()
+            except OSError:
+                # if the stat failed, it could have been due to a
+                # broken symlink. in any case, return the entry
+                # without the stat info. a follow up stat request by
+                # the client can verify if the path is truly gone or
+                # if it's a broken link
+                return x.name
+            else:
+                return (x.name, self._fs_stat_to_fuse_attrs(st), 0)
+
+        return list(itertools.chain(['.', '..'], map(transform_entry, f)))
 
     def releasedir(self, path: typing.Optional[str], fh: int) -> int:
         # NB: fusepy ignores raw_fi in this method for some reason
         self._delete_dir(fh).close()
         return 0
 
     def unlink(self, path: str) -> int:
```

### Comparing `userspacefs-3.0.0/userspacefs/fusepy.py` & `userspacefs-3.1.0/userspacefs/fusepy.py`

 * *Files identical despite different names*

### Comparing `userspacefs-3.0.0/userspacefs/macos_path_conversion.py` & `userspacefs-3.1.0/userspacefs/macos_path_conversion.py`

 * *Files identical despite different names*

### Comparing `userspacefs-3.0.0/userspacefs/memoryfs.py` & `userspacefs-3.1.0/userspacefs/memoryfs.py`

 * *Files identical despite different names*

### Comparing `userspacefs-3.0.0/userspacefs/path_common.py` & `userspacefs-3.1.0/userspacefs/path_common.py`

 * *Files 5% similar despite different names*

```diff
@@ -21,14 +21,19 @@
 from collections.abc import Sequence, Callable, Iterable
 
 import userspacefs.abc as fsabc
 
 def is_parent(path_a: fsabc.Path, path_b: fsabc.Path) -> bool:
     return path_a in path_b.parents
 
+def join_name(path_a: fsabc.Path, *names: str) -> fsabc.Path:
+    for p in names:
+        path_a = path_a.joinpath("_").with_name(p)
+    return path_a
+
 # NB: this acts like a pathlib PurePath object
 class Path(object):
     def __init__(self, compsi: Iterable[str], fn_norm: typing.Optional[Callable[[str], str]] = None):
         comps = tuple(compsi)
         assert all(type(comp) is str for comp in comps)
         self._comps = comps
         if fn_norm is None:
@@ -48,16 +53,16 @@
 
     def joinpath(self, *comps: str) -> typing.Self:
         assert all(a for a in comps), "empty path components are  not allowed!"
         return self.__class__(itertools.chain(self._comps, comps),
                               fn_norm=self._fn_norm)
 
     @property
-    def parts(self) -> tuple[str]:
-        return typing.cast(typing.Tuple[str], tuple(itertools.chain(('/',), self._comps)))
+    def parts(self) -> tuple[str, ...]:
+        return typing.cast(typing.Tuple[str, ...], tuple(itertools.chain(('/',), self._comps)))
 
     # NB: This is probably an evil abuse of the '/' operator
     def __truediv__(self, elt: str) -> typing.Self:
         return self.joinpath(elt)
 
     def __repr__(self) -> str:
         return 'Path' + str(self)
@@ -98,8 +103,10 @@
             p = n
         return ret
 
     def normed(self) -> typing.Self:
         return type(self)(self._norm(), fn_norm=self._fn_norm)
 
     def with_name(self, new_name: str) -> typing.Self:
+        if '/' in new_name:
+            raise ValueError("Invalid name %r" % (new_name,))
         return self.parent / new_name
```

### Comparing `userspacefs-3.0.0/userspacefs/smbserver.py` & `userspacefs-3.1.0/userspacefs/smbserver.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,15 +37,16 @@
 from concurrent.futures import ThreadPoolExecutor
 from datetime import datetime, timezone
 
 from typing_extensions import TypedDict
 
 import userspacefs.abc as fsabc
 
-from userspacefs.util_dumpster import datetime_now, OldStat, OldDirectory, trans, SharedLock, ConnPool
+from userspacefs.util_dumpster import datetime_now, OldStat, OldDirectory, trans, SharedLock, ConnPool, DummyStat
+from userspacefs.path_common import join_name
 
 log = logging.getLogger(__name__)
 
 T = typing.TypeVar('T')
 
 def _check_methods(C: typing.Type[typing.Any], *methods: str) -> bool:
     mro = C.__mro__
@@ -2644,30 +2645,40 @@
                              cs: SMBClientHandler,
                              backend: AsyncBackend,
                              req: SMBMessage) -> SMBMessage:
     async def smb_path_to_fs_path(path: str) -> fsabc.Path:
         comps = path[1:].split("\\")
         if comps and not comps[-1]:
             comps.pop()
-        return (await fs.create_path(*comps))
+        return join_name((await fs.create_path()), *comps)
 
     def normalize_stat(stat: OldStat) -> NormalStat:
         birthtime = getattr(stat, "birthtime", datetime.fromtimestamp(0, tz=timezone.utc))
         mtime = getattr(stat, "mtime", birthtime)
         ctime = getattr(stat, "ctime", mtime)
         atime = getattr(stat, "atime", ctime)
 
         type = getattr(stat, "type")
         size = getattr(stat, "size")
 
         return NormalStat(birthtime, mtime, ctime, atime, type, size)
 
     async def normalize_dir_entry(entry: JustNameDirStat) -> NormalStat:
         # TODO: use new dir entry interface so we can call .stat() on it
-        to_normalize = OldStat((await fs.stat(path / entry.name)))
+        st: fsabc.Stat
+        try:
+            st = await fs.stat(path / entry.name)
+        except OSError:
+            # NB: either dir entry went missing, or it's behaving like a
+            #     broken symlink. we just replace it with a dummy stat. if
+            #     the client wants more info, they can issue a direct stat. we
+            #     do this to allow the client to delete the file in case it's
+            #     like a broken symlink.
+            st = DummyStat()
+        to_normalize = OldStat(st)
         return normalize_stat(to_normalize)
 
     def verify_andx(req: SMBMessage) -> None:
         pass
 
     parameters: SMBParameters
     data: SMBData
@@ -2888,15 +2899,15 @@
 
                     is_directory_search = comps[-1] in ["*", "*.*", ""]
                     if is_directory_search:
                         comps = comps[:-1]
 
                 buffered_entries: typing.List[typing.Tuple[str, NormalStat]]
                 buffered_entries_idx: int
-                path = await fs.create_path(*comps)
+                path = join_name((await fs.create_path()), *comps)
                 try:
                     if is_directory_search:
                         handle = await fs.old_open_directory(path)
 
                         entry: typing.Optional[typing.Tuple[str, NormalStat]]
                         entry = None
                         next_entry: typing.Optional[typing.Tuple[str, NormalStat]]
```

### Comparing `userspacefs-3.0.0/userspacefs/stdlibfs.py` & `userspacefs-3.1.0/userspacefs/stdlibfs.py`

 * *Files 17% similar despite different names*

```diff
@@ -16,16 +16,19 @@
 # along with userspacefs.  If not, see <http://www.gnu.org/licenses/>.
 
 import userspacefs.abc as fsabc
 
 from userspacefs import simple_main_from_argv
 
 import datetime
+import errno
 import io
+import itertools
 import os
+import os.path
 import sys
 import time
 import typing
 
 from collections.abc import Callable, Sequence
 from pathlib import PurePath as Path
 
@@ -39,33 +42,46 @@
 class FileSystem(fsabc.FileSystemG[Path, File]):
     def __init__(self, root: str):
         self._root = Path(root)
 
     def create_path(self, *parts: str) -> Path:
         return self._root.joinpath(*parts)
 
+    def _check_path(self, path: Path) -> None:
+        # path components are taken as literals
+        # i.e., ".." and "." have no special meaning.
+        # if we pass them to the os functions, they will be interpreted
+        # in a special way. since no file can exist with those names,
+        # if we detect them, return ENOENT
+        if (".." in path.parts or
+            "." in path.parts):
+            raise OSError(errno.ENOENT, os.strerror(errno.ENOENT))
+
     def fstat(self, file: File) -> os.stat_result:
         return os.fstat(file.fileno())
 
     def close(self) -> None:
         pass
 
     def fsync(self, file: File) -> None:
         return os.fsync(file.fileno())
 
     def mkdir(self, path: Path) -> None:
+        self._check_path(path)
         return os.mkdir(path)
 
     def open(self, path: Path, mode: int) -> File:
+        self._check_path(path)
         return typing.cast(
             File,
             os.fdopen(os.open(path, mode), "r+b", buffering=0),
         )
 
     def open_directory(self, path: Path) -> fsabc.Directory:
+        self._check_path(path)
         return os.scandir(path)
 
     def preadinto(self, file: File, buf: fsabc.Buffer, offset: int) -> int:
         if hasattr(os, 'preadv'):
             return os.preadv(file.fileno(), [buf], offset)
         else:
             with memoryview(buf) as mbuf:
@@ -74,27 +90,32 @@
                 mbuf[:len(data)] = data
                 return len(data)
 
     def pwrite(self, file: File, data: fsabc.Buffer, offset: int) -> int:
         return os.pwrite(file.fileno(), data, offset)
 
     def replace(self, source: Path, dest: Path) -> None:
+        self._check_path(source)
+        self._check_path(dest)
         os.replace(source, dest)
 
     def rmdir(self, path: Path) -> None:
+        self._check_path(path)
         os.rmdir(path)
 
     def stat(self, path: Path) -> os.stat_result:
+        self._check_path(path)
         return os.stat(path)
 
     def statvfs(self) -> fsabc.StatVFS:
         # TODO: Windows support
         return os.statvfs(self._root)
 
     def unlink(self, path: Path) -> None:
+        self._check_path(path)
         os.unlink(path)
 
     def futimes(self, file: File,
                 times: typing.Optional[typing.Tuple[float, float]] = None) -> None:
         # TODO: Windows support
         os.utime(file.fileno(), times=times)
```

### Comparing `userspacefs-3.0.0/userspacefs/util_dumpster.py` & `userspacefs-3.1.0/userspacefs/util_dumpster.py`

 * *Files 3% similar despite different names*

```diff
@@ -66,14 +66,35 @@
         ...
 
 class OldDirectoryProtocol(Iterator[OldDirStatProtocol], typing.Protocol):
     @abstractmethod
     def close(self) -> None:
         ...
 
+class DummyStat(fsabc.Stat):
+    @property
+    def st_size(self) -> int:
+        return 0
+
+    @property
+    def st_mode(self) -> int:
+        return stat.S_IFREG
+
+    @property
+    def st_mtime_ns(self) -> int:
+        return 0
+
+    @property
+    def st_atime_ns(self) -> int:
+        return 0
+
+    @property
+    def st_ctime_ns(self) -> int:
+        return 0
+
 class NewStat(fsabc.Stat):
     def __init__(self, old_st: OldStatProtocol):
         self._st = old_st
 
     @property
     def st_size(self) -> int:
         return self._st.size
```

### Comparing `userspacefs-3.0.0/userspacefs/webdavserver.py` & `userspacefs-3.1.0/userspacefs/webdavserver.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,17 +13,17 @@
 # GNU General Public License for more details.
 
 # You should have received a copy of the GNU General Public License
 # along with userspacefs.  If not, see <http://www.gnu.org/licenses/>.
 
 import userspacefs.abc as fsabc
 
-from userspacefs.path_common import is_parent
+from userspacefs.path_common import is_parent, join_name
 from userspacefs.smbserver import AsyncWorkerPool, AsyncFS, AsyncFile, cant_fail, JustNameDirStat
-from userspacefs.util_dumpster import OldStat, datetime_from_ts
+from userspacefs.util_dumpster import OldStat, datetime_from_ts, DummyStat
 
 from aiohttp import web
 
 import asyncio
 import contextlib
 import datetime
 import dataclasses as dc
@@ -65,15 +65,25 @@
 
     type = getattr(stat, "type")
     size = getattr(stat, "size")
 
     return NormalStat(birthtime, mtime, ctime, atime, type, size)
 
 async def normalize_dir_entry(fs: AsyncFS, path: fsabc.Path, entry: JustNameDirStat) -> NormalStat:
-    to_normalize = OldStat((await fs.stat(path / entry.name)))
+    st: fsabc.Stat
+    try:
+        st = await fs.stat(path / entry.name)
+    except OSError:
+        # NB: either dir entry went missing, or it's behaving like a
+        #     broken symlink. we just replace it with a dummy stat. if
+        #     the client wants more info, they can issue a direct stat. we
+        #     do this to allow the client to delete the file in case it's
+        #     like a broken symlink.
+        st = DummyStat()
+    to_normalize = OldStat(st)
     return normalize_stat(to_normalize)
 
 @dc.dataclass
 class WebDAVLock:
     timeout: typing.Optional[int]
     path: fsabc.Path
     token: str
@@ -95,15 +105,15 @@
     parts = parts[len(ctx.path_root_parts):]
     return parts
 
 async def path_from_url_path(ctx: WebDAVServerCtx, ipath: str) -> fsabc.Path:
     parts = get_rel_path_parts(ctx, ipath)
     if parts and not parts[-1]:
         parts.pop()
-    path = await ctx.fs.create_path(*map(urllib.parse.unquote, parts))
+    path = join_name((await ctx.fs.create_path()), *map(urllib.parse.unquote, parts))
     return path
 
 async def path_from_req(ctx: WebDAVServerCtx,
                         req: web.Request) -> fsabc.Path:
     p = await path_from_url_path(ctx, req.url.raw_path)
     return p
```

### Comparing `userspacefs-3.0.0/userspacefs.egg-info/PKG-INFO` & `userspacefs-3.1.0/userspacefs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: userspacefs
-Version: 3.0.0
+Version: 3.1.0
 Summary: Cross-platform user-space file systems for Python
 Home-page: https://thelig.ht/code/userspacefs
 Author: Rian Hunter
 Author-email: rian@alum.mit.edu
 License: GPL3
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3
```

### Comparing `userspacefs-3.0.0/userspacefs.egg-info/SOURCES.txt` & `userspacefs-3.1.0/userspacefs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

