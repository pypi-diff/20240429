# Comparing `tmp/dbxfs-2.0.0.tar.gz` & `tmp/dbxfs-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbxfs-2.0.0.tar", last modified: Fri Jan  5 19:05:57 2024, max compression
+gzip compressed data, was "dbxfs-2.0.1.tar", last modified: Mon Apr 29 15:36:02 2024, max compression
```

## Comparing `dbxfs-2.0.0.tar` & `dbxfs-2.0.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 rian      (1000) rian      (1000)        0 2024-01-05 19:05:57.452662 dbxfs-2.0.0/
--rw-r--r--   0 rian      (1000) rian      (1000)    35441 2023-04-02 05:01:39.000000 dbxfs-2.0.0/LICENSE
--rw-r--r--   0 rian      (1000) rian      (1000)       16 2018-11-06 22:09:00.000000 dbxfs-2.0.0/MANIFEST.in
--rw-r--r--   0 rian      (1000) rian      (1000)     3344 2024-01-05 19:05:57.452662 dbxfs-2.0.0/PKG-INFO
--rw-r--r--   0 rian      (1000) rian      (1000)     2888 2024-01-05 18:51:24.000000 dbxfs-2.0.0/README.md
-drwxr-xr-x   0 rian      (1000) rian      (1000)        0 2024-01-05 19:05:57.452662 dbxfs-2.0.0/dbxfs/
--rw-r--r--   0 rian      (1000) rian      (1000)      666 2018-10-03 00:17:59.000000 dbxfs-2.0.0/dbxfs/__init__.py
--rw-r--r--   0 rian      (1000) rian      (1000)    83670 2024-01-05 01:15:05.000000 dbxfs-2.0.0/dbxfs/cachingfs.py
--rw-r--r--   0 rian      (1000) rian      (1000)    44654 2023-12-31 19:40:35.000000 dbxfs-2.0.0/dbxfs/dbxfs.py
--rw-r--r--   0 rian      (1000) rian      (1000)     4654 2024-01-05 01:15:05.000000 dbxfs-2.0.0/dbxfs/disable_quick_look.py
--rw-r--r--   0 rian      (1000) rian      (1000)     5869 2024-01-05 18:51:24.000000 dbxfs-2.0.0/dbxfs/gui.py
--rwxr-xr-x   0 rian      (1000) rian      (1000)    31949 2024-01-05 18:51:24.000000 dbxfs-2.0.0/dbxfs/main.py
--rw-r--r--   0 rian      (1000) rian      (1000)        0 2023-11-15 23:06:10.000000 dbxfs-2.0.0/dbxfs/py.typed
--rw-r--r--   0 rian      (1000) rian      (1000)     8610 2023-12-30 21:18:32.000000 dbxfs-2.0.0/dbxfs/safefs_glue.py
--rw-r--r--   0 rian      (1000) rian      (1000)     5141 2023-12-30 21:18:32.000000 dbxfs-2.0.0/dbxfs/translate_ignored_files.py
--rw-r--r--   0 rian      (1000) rian      (1000)     4477 2023-12-30 21:18:31.000000 dbxfs-2.0.0/dbxfs/util_dumpster.py
--rw-r--r--   0 rian      (1000) rian      (1000)      689 2018-10-03 00:15:24.000000 dbxfs-2.0.0/dbxfs/version.py
-drwxr-xr-x   0 rian      (1000) rian      (1000)        0 2024-01-05 19:05:57.452662 dbxfs-2.0.0/dbxfs.egg-info/
--rw-r--r--   0 rian      (1000) rian      (1000)     3344 2024-01-05 19:05:57.000000 dbxfs-2.0.0/dbxfs.egg-info/PKG-INFO
--rw-r--r--   0 rian      (1000) rian      (1000)      440 2024-01-05 19:05:57.000000 dbxfs-2.0.0/dbxfs.egg-info/SOURCES.txt
--rw-r--r--   0 rian      (1000) rian      (1000)        1 2024-01-05 19:05:57.000000 dbxfs-2.0.0/dbxfs.egg-info/dependency_links.txt
--rw-r--r--   0 rian      (1000) rian      (1000)       42 2024-01-05 19:05:57.000000 dbxfs-2.0.0/dbxfs.egg-info/entry_points.txt
--rw-r--r--   0 rian      (1000) rian      (1000)      173 2024-01-05 19:05:57.000000 dbxfs-2.0.0/dbxfs.egg-info/requires.txt
--rw-r--r--   0 rian      (1000) rian      (1000)        6 2024-01-05 19:05:57.000000 dbxfs-2.0.0/dbxfs.egg-info/top_level.txt
--rw-r--r--   0 rian      (1000) rian      (1000)       73 2024-01-05 19:05:57.452662 dbxfs-2.0.0/setup.cfg
--rw-r--r--   0 rian      (1000) rian      (1000)     1935 2024-01-05 18:54:33.000000 dbxfs-2.0.0/setup.py
+drwxr-xr-x   0 rian      (1000) rian      (1000)        0 2024-04-29 15:36:02.534302 dbxfs-2.0.1/
+-rw-r--r--   0 rian      (1000) rian      (1000)    35441 2023-04-02 05:01:39.000000 dbxfs-2.0.1/LICENSE
+-rw-r--r--   0 rian      (1000) rian      (1000)       16 2018-11-06 22:09:00.000000 dbxfs-2.0.1/MANIFEST.in
+-rw-r--r--   0 rian      (1000) rian      (1000)     3343 2024-04-29 15:36:02.534302 dbxfs-2.0.1/PKG-INFO
+-rw-r--r--   0 rian      (1000) rian      (1000)     2887 2024-01-09 19:10:32.000000 dbxfs-2.0.1/README.md
+drwxr-xr-x   0 rian      (1000) rian      (1000)        0 2024-04-29 15:36:02.534302 dbxfs-2.0.1/dbxfs/
+-rw-r--r--   0 rian      (1000) rian      (1000)      666 2018-10-03 00:17:59.000000 dbxfs-2.0.1/dbxfs/__init__.py
+-rw-r--r--   0 rian      (1000) rian      (1000)    83799 2024-01-11 23:32:25.000000 dbxfs-2.0.1/dbxfs/cachingfs.py
+-rw-r--r--   0 rian      (1000) rian      (1000)    44654 2023-12-31 19:40:35.000000 dbxfs-2.0.1/dbxfs/dbxfs.py
+-rw-r--r--   0 rian      (1000) rian      (1000)     4654 2024-01-05 01:15:05.000000 dbxfs-2.0.1/dbxfs/disable_quick_look.py
+-rw-r--r--   0 rian      (1000) rian      (1000)     5869 2024-01-05 19:12:38.000000 dbxfs-2.0.1/dbxfs/gui.py
+-rwxr-xr-x   0 rian      (1000) rian      (1000)    29481 2024-04-29 15:28:59.000000 dbxfs-2.0.1/dbxfs/main.py
+-rw-r--r--   0 rian      (1000) rian      (1000)        0 2023-11-15 23:06:10.000000 dbxfs-2.0.1/dbxfs/py.typed
+-rw-r--r--   0 rian      (1000) rian      (1000)     8610 2023-12-30 21:18:32.000000 dbxfs-2.0.1/dbxfs/safefs_glue.py
+-rw-r--r--   0 rian      (1000) rian      (1000)     5143 2024-04-29 15:23:28.000000 dbxfs-2.0.1/dbxfs/translate_ignored_files.py
+-rw-r--r--   0 rian      (1000) rian      (1000)     4477 2023-12-30 21:18:31.000000 dbxfs-2.0.1/dbxfs/util_dumpster.py
+-rw-r--r--   0 rian      (1000) rian      (1000)      689 2018-10-03 00:15:24.000000 dbxfs-2.0.1/dbxfs/version.py
+drwxr-xr-x   0 rian      (1000) rian      (1000)        0 2024-04-29 15:36:02.534302 dbxfs-2.0.1/dbxfs.egg-info/
+-rw-r--r--   0 rian      (1000) rian      (1000)     3343 2024-04-29 15:36:02.000000 dbxfs-2.0.1/dbxfs.egg-info/PKG-INFO
+-rw-r--r--   0 rian      (1000) rian      (1000)      440 2024-04-29 15:36:02.000000 dbxfs-2.0.1/dbxfs.egg-info/SOURCES.txt
+-rw-r--r--   0 rian      (1000) rian      (1000)        1 2024-04-29 15:36:02.000000 dbxfs-2.0.1/dbxfs.egg-info/dependency_links.txt
+-rw-r--r--   0 rian      (1000) rian      (1000)       42 2024-04-29 15:36:02.000000 dbxfs-2.0.1/dbxfs.egg-info/entry_points.txt
+-rw-r--r--   0 rian      (1000) rian      (1000)      173 2024-04-29 15:36:02.000000 dbxfs-2.0.1/dbxfs.egg-info/requires.txt
+-rw-r--r--   0 rian      (1000) rian      (1000)        6 2024-04-29 15:36:02.000000 dbxfs-2.0.1/dbxfs.egg-info/top_level.txt
+-rw-r--r--   0 rian      (1000) rian      (1000)       73 2024-04-29 15:36:02.534302 dbxfs-2.0.1/setup.cfg
+-rw-r--r--   0 rian      (1000) rian      (1000)     1935 2024-04-29 15:35:51.000000 dbxfs-2.0.1/setup.py
```

### Comparing `dbxfs-2.0.0/LICENSE` & `dbxfs-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dbxfs-2.0.0/PKG-INFO` & `dbxfs-2.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbxfs
-Version: 2.0.0
+Version: 2.0.1
 Summary: User-space file system for Dropbox
 Home-page: https://thelig.ht/code/dbxfs
 Author: Rian Hunter
 Author-email: rian@alum.mit.edu
 License: GPL3
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3
@@ -53,15 +53,15 @@
 `fuse`.
 
 Run the following command:
 
     $ pip3 install dbxfs
 
 On Arch Linux and derivatives, you can find it in the AUR as
-[dbxfs](https://aur.archlinux.org/packages/dbxfs>).
+[dbxfs](https://aur.archlinux.org/packages/dbxfs).
 
 Usage
 -----
 
 Use `dbxfs` like you would use the `mount` command:
 
     $ dbxfs <mount_point>
```

### Comparing `dbxfs-2.0.0/README.md` & `dbxfs-2.0.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 `fuse`.
 
 Run the following command:
 
     $ pip3 install dbxfs
 
 On Arch Linux and derivatives, you can find it in the AUR as
-[dbxfs](https://aur.archlinux.org/packages/dbxfs>).
+[dbxfs](https://aur.archlinux.org/packages/dbxfs).
 
 Usage
 -----
 
 Use `dbxfs` like you would use the `mount` command:
 
     $ dbxfs <mount_point>
```

### Comparing `dbxfs-2.0.0/dbxfs/__init__.py` & `dbxfs-2.0.1/dbxfs/__init__.py`

 * *Files identical despite different names*

### Comparing `dbxfs-2.0.0/dbxfs/cachingfs.py` & `dbxfs-2.0.1/dbxfs/cachingfs.py`

 * *Files 1% similar despite different names*

```diff
@@ -388,16 +388,16 @@
                     #
                     #     We choose 2) because cache entries for directories don't really
                     #     store any interesting info aside from the fact that they are a directory.
 
                     cursor.execute("select md from md_cache where path_key = ?", (path_key,))
                     mdrow = cursor.fetchone()
                     if mdrow is None:
-                        st = Stat(mtime=datenow_now(), type='directory', size=0,
-                                  id=None, ctime=datenow_now(), rev=None, attrs={})
+                        st = Stat(mtime=datetime_now(), type='directory', size=0,
+                                  id=None, ctime=datetime_now(), rev=None, attrs={})
                         fs._update_md(cursor, path, st)
                     else:
                         assert mdrow[0] is not None and json_to_stat(mdrow[0]).type == 'directory'
 
                     # this only inserts EMPTY_DIR_ENT, the rest is filled
                     # by _update_md()
                     cursor.executemany("INSERT INTO md_cache_entries "
@@ -521,20 +521,28 @@
         assert not err
         ret = WriteFile(handle, bufp.value, bufsize.value, ctypes.byref(bytes_written), ctypes.byref(overlapped))
         if not ret:
             raise ctypes.WinError(descr="Failed to call WriteFile()")
 
         return bytes_written.value
 else:
-    def os_preadinto(fd: int, data: bytearray | memoryview, offset: int) -> int:
+    def os_preadinto_pread(fd: int, data: bytearray | memoryview, offset: int) -> int:
         size = len(data)
         ret = os.pread(fd, size, offset)
         data[:len(ret)] = ret
         return len(ret)
 
+    def os_preadinto_preadv(fd: int, data: bytearray | memoryview, offset: int) -> int:
+        return os.preadv(fd, [data], offset)
+
+    if hasattr(os, 'preadv'):
+        os_preadinto = os_preadinto_preadv
+    else:
+        os_preadinto = os_preadinto_pread
+
     os_pwrite = os.pwrite
 
 class PreadMixin(object):
     def pread(self, size, offset):
         buf = bytearray(size)
         amt = self.preadinto(buf, offset)
         return memoryview(buf)[:amt]
@@ -658,18 +666,15 @@
                     except Exception as e:
                         if not (isinstance(e, (OSError, IOError)) and
                                 e.errno == errno.ENOSPC):
                             log.warning("Failed to cache data", exc_info=True)
 
                     return amt
 
-                if hasattr(os, 'preadv'):
-                    return os.preadv(self.cached_file.fileno(), [data], offset)
-                else:
-                    return os_preadinto(self.cached_file.fileno(), data, offset)
+                return os_preadinto(self.cached_file.fileno(), data, offset)
 
     def close(self):
         th = None
         with self.reset_lock:
             if self.is_closed:
                 return
             self.is_closed = True
@@ -1806,15 +1811,15 @@
 
     def file_name_norm(self, fn):
         return self._fs.file_name_norm(fn)
 
     def _invalidate_path(self, path):
         with self._get_db_conn() as conn, \
              trans(conn, self._db_lock, is_exclusive=True), contextlib.closing(conn.cursor()) as cursor:
-            self._invalidate_entry(cursor, path)
+            self._invalidate_entry(cursor, path.normed())
 
     def open(self, path, mode=os.O_RDONLY, directory=False):
         with self._file_cache_lock:
             self._openners += 1
         try:
             try:
                 st = self._stat(path)
```

### Comparing `dbxfs-2.0.0/dbxfs/dbxfs.py` & `dbxfs-2.0.1/dbxfs/dbxfs.py`

 * *Files identical despite different names*

### Comparing `dbxfs-2.0.0/dbxfs/disable_quick_look.py` & `dbxfs-2.0.1/dbxfs/disable_quick_look.py`

 * *Files identical despite different names*

### Comparing `dbxfs-2.0.0/dbxfs/gui.py` & `dbxfs-2.0.1/dbxfs/gui.py`

 * *Files identical despite different names*

### Comparing `dbxfs-2.0.0/dbxfs/main.py` & `dbxfs-2.0.1/dbxfs/main.py`

 * *Files 8% similar despite different names*

```diff
@@ -88,60 +88,61 @@
 
 HOLD_MUTEX = None
 
 def acquire_hold(instance_guid):
     # this is only implemented for windows currently
     if sys.platform != 'win32':
         return True
+    else:
 
-    import win32api
-    import win32event
-    import winerror
-
-    global HOLD_MUTEX
-    HOLD_MUTEX = win32event.CreateMutex(None, True, instance_guid)
-    le = win32api.GetLastError()
-    log.debug("Last error: %r, instance: %r", le, instance_guid)
-    return le != winerror.ERROR_ALREADY_EXISTS
+        import win32api
+        import win32event
+        import winerror
+
+        global HOLD_MUTEX
+        HOLD_MUTEX = win32event.CreateMutex(None, True, instance_guid)
+        le = win32api.GetLastError()
+        log.debug("Last error: %r, instance: %r", le, instance_guid)
+        return le != winerror.ERROR_ALREADY_EXISTS
 
 def allow_multiple(instance_guid, use_gui):
     # if we're not running frozen, the user presumably knows what they
     # are doing, so we permit multiple instances
     if not getattr(sys, 'frozen', False):
         return True
 
     # this is only implemented for windows currently
     if sys.platform != 'win32':
         return True
+    else:
+        import win32gui
+        import win32com.client
 
-    import win32gui
-    import win32com.client
-
-    def get_disks():
-        strComputer = "."
-        objWMIService = win32com.client.Dispatch("WbemScripting.SWbemLocator")
-        objSWbemServices = objWMIService.ConnectServer(strComputer, "root\\cimv2")
-        colItems = objSWbemServices.ExecQuery("Select * from Win32_LogicalDisk")
-        return colItems
-
-    # create mutex with guid
-    if not acquire_hold(instance_guid):
-        if use_gui:
-            win = win32gui.FindWindow(None, "dbxfs")
-            if win:
-                win32gui.SetForegroundWindow(win)
+        def get_disks():
+            strComputer = "."
+            objWMIService = win32com.client.Dispatch("WbemScripting.SWbemLocator")
+            objSWbemServices = objWMIService.ConnectServer(strComputer, "root\\cimv2")
+            colItems = objSWbemServices.ExecQuery("Select * from Win32_LogicalDisk")
+            return colItems
+
+        # create mutex with guid
+        if not acquire_hold(instance_guid):
+            if use_gui:
+                win = win32gui.FindWindow(None, "dbxfs")
+                if win:
+                    win32gui.SetForegroundWindow(win)
+                else:
+                    for disk in get_disks():
+                        if disk.ProviderName is not None and disk.ProviderName.endswith("\\dbxfs"):
+                            subprocess.run(["start", disk.name], shell=True)
             else:
-                for disk in get_disks():
-                    if disk.ProviderName is not None and disk.ProviderName.endswith("\\dbxfs"):
-                        subprocess.run(["start", disk.name], shell=True)
-        else:
-            print("Another instance already running")
-        return False
+                print("Another instance already running")
+            return False
 
-    return True
+        return True
 
 def yes_no_input(message: typing.Optional[str] = None,
                  default_yes: bool = False) -> bool:
     if default_yes:
         extra = "[Y/n]"
     else:
         extra = "[y/N]"
@@ -155,14 +156,22 @@
 
 class UIProtocol(typing.Protocol):
     @abstractmethod
     def can_interact(self) -> bool:
         ...
 
     @abstractmethod
+    def warning(self, message: str) -> None:
+        ...
+
+    @abstractmethod
+    def error(self, message: str) -> None:
+        ...
+
+    @abstractmethod
     def yes_no_input(self, message: typing.Optional[str] = None,
                      default_yes: bool = False) -> bool:
         ...
 
     @abstractmethod
     def link_dbxfs(self, authorize_url: str) -> str:
         ...
@@ -410,69 +419,14 @@
                 ui.warning("dbxfs is out of date (%s vs %s), upgrade with 'pip3 install --upgrade dbxfs'" %
                            (rversion, version))
     except Exception:
         log.warning("Failed to get most recent version", exc_info=True)
 
     return (save_config, False)
 
-class FUSEOption(argparse.Action):
-    def __init__(self, **kw):
-        super(FUSEOption, self).__init__(**kw)
-
-    def __call__(self,
-                 parser: argparse.ArgumentParser,
-                 ns: argparse.Namespace,
-                 values: str | Sequence[typing.Any] | None,
-                 option_string: str | None = None) -> None:
-        if ns.o is None:
-            ns.o = {}
-        assert isinstance(values, str)
-        for kv in values.split(","):
-            ret = kv.split("=", 1)
-            if len(ret) == 2:
-                ns.o[ret[0]] = ret[1]
-            else:
-                ns.o[ret[0]] = True
-
-def add_cli_arguments(parser: argparse.ArgumentParser) -> None:
-    def ensure_listen_address(string: str) -> typing.Tuple[str, int]:
-        try:
-            (host, ports) = string.split(":", 1)
-        except ValueError:
-            host = string
-            port = 0
-        else:
-            port = int(ports)
-            if not (0 <= port < 65536):
-                raise argparse.ArgumentTypeError("%r is not a valid TCP port" % (port,))
-
-        if not host:
-            host = "127.0.0.1"
-
-        return (host, port)
-
-    parser.add_argument("-f", "--foreground", action="store_true",
-                        help="keep filesystem server in foreground")
-    parser.add_argument("-v", "--verbose", action="count", default=0,
-                        help="show log messages, use twice for maximum verbosity")
-    _group = parser.add_mutually_exclusive_group()
-    _group.add_argument("-s", "--smb", action="store_true",
-                        help="force mounting via SMB")
-    _group.add_argument("-w", "--webdav", action="store_true",
-                        help="force mounting via WebDAV")
-    parser.add_argument("-n", "--no-mount", action="store_true",
-                        dest="smb_no_mount",
-                        help="export filesystem via network server but don't mount it")
-    parser.add_argument("-l", "--listen-address",
-                        dest="smb_listen_address",
-                        type=ensure_listen_address,
-                        help="address that the filesystem server should listen on, append colon to specify port")
-    parser.add_argument("-o", metavar='opt,[opt...]', action=FUSEOption,
-                        help="FUSE options, e.g. -o uid=1000,allow_other")
-
 def _main(argv: typing.Optional[typing.List[str]] = None):
     try:
         import pyi_splash
 
         # Close the splash screen. It does not matter when the call
         # to this function is made, the splash screen remains open until
         # this function is called or the Python program is terminated.
@@ -495,32 +449,31 @@
     # Protect access token and potentially encryption keys
     my_block_tracing()
 
     if argv is None:
         argv = sys.argv
 
     parser = argparse.ArgumentParser()
-    add_cli_arguments(parser)
+    userspacefs.add_simple_cli_arguments(parser)
+    parser.add_argument("-v", "--verbose", action="count", default=0,
+                        help="show log messages, use twice for maximum verbosity")
     parser.add_argument("-c", "--config-file",
                         help="config file path")
     parser.add_argument("--print-default-config-file", action='store_true',
                         help="print default config file path to standard out and quit")
     parser.add_argument("--get-refresh-token", action='store_true',
                         help="authorize new refresh token and print to standard out")
     parser.add_argument("--gui", action='store_true',
                         help="Use GUI for interactive configuration")
     parser.add_argument("--userspacefs-main", action='store_true',
                         help=argparse.SUPPRESS)
     parser.add_argument("mount_point", nargs='?')
     args = parser.parse_args(argv[1:])
 
-    if args.smb_no_mount and not args.smb and not args.webdav:
-        print("error: either --smb or --webdav must be specified when --no-mount is specified",
-              file=sys.stderr)
-        return -1
+    userspacefs.check_simple_args_result(parser, args)
 
     if args.userspacefs_main:
         return userspacefs.main(argv)
 
     if sys.stderr is None:
         logging_stream = headless_stream_handler(APP_NAME)
     else:
@@ -605,15 +558,15 @@
         cache_folder = config.get("cache_dir")
 
         mount_point = args.mount_point
         if mount_point is None:
             mount_point = config.get("mount_point")
 
         # NB: mount point is always optional for windows because we can auto-generate one
-        if not args.smb_no_mount and mount_point is None and sys.platform != 'win32':
+        if not args.no_mount and mount_point is None and sys.platform != 'win32':
             parser.print_usage()
             print("%s: error: please provide the mount_point argument" % (os.path.basename(argv[0]),))
             return 1
 
         encrypted_folders = config.get("encrypted_folders", [])
 
         if refresh_token is None and access_token is None:
@@ -841,25 +794,23 @@
         main_executable = None
 
     # we don't want the installer to display the splash when
     # launching the file system server process. This is our custom
     # extension
     os.environ['PYINSTALLER_NOSPLASH'] = '1'
 
-    return userspacefs.simple_main(mount_point, display_name,
-                                   ('dbxfs.main.create_fs', fs_args),
-                                   on_new_process=('dbxfs.main.on_new_process', proc_args),
-                                   on_mount=('dbxfs.main.on_mount', on_mount_args),
-                                   foreground=args.foreground,
-                                   smb_only=args.smb,
-                                   webdav_only=args.webdav,
-                                   no_mount=args.smb_no_mount,
-                                   listen_address=args.smb_listen_address,
-                                   fuse_options=args.o,
-                                   main_executable=main_executable)
+    return userspacefs.simple_main_with_args(
+        mount_point,
+        display_name,
+        ('dbxfs.main.create_fs', fs_args),
+        args,
+        on_new_process=('dbxfs.main.on_new_process', proc_args),
+        on_mount=('dbxfs.main.on_mount', on_mount_args),
+        main_executable=main_executable,
+    )
 
 def main(argv: typing.Optional[typing.List[str]] = None):
     try:
         return _main(argv)
     except KeyboardInterrupt:
         return 1
```

### Comparing `dbxfs-2.0.0/dbxfs/safefs_glue.py` & `dbxfs-2.0.1/dbxfs/safefs_glue.py`

 * *Files identical despite different names*

### Comparing `dbxfs-2.0.0/dbxfs/translate_ignored_files.py` & `dbxfs-2.0.1/dbxfs/translate_ignored_files.py`

 * *Files 1% similar despite different names*

```diff
@@ -146,15 +146,15 @@
                         path=[decode_name(p)
                               for p in entry.path]
                     )
                 )
 
             return cb(toret)
 
-        return self._sub.create_watch(newcb, *n, **kw)
+        return self._sub.x_create_watch(newcb, *n, **kw)
 
     def close(self):
         return self._sub.close()
 
     def create_path(self, *args):
         return self._sub.create_path(*args)
```

### Comparing `dbxfs-2.0.0/dbxfs/util_dumpster.py` & `dbxfs-2.0.1/dbxfs/util_dumpster.py`

 * *Files identical despite different names*

### Comparing `dbxfs-2.0.0/dbxfs/version.py` & `dbxfs-2.0.1/dbxfs/version.py`

 * *Files identical despite different names*

### Comparing `dbxfs-2.0.0/dbxfs.egg-info/PKG-INFO` & `dbxfs-2.0.1/dbxfs.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbxfs
-Version: 2.0.0
+Version: 2.0.1
 Summary: User-space file system for Dropbox
 Home-page: https://thelig.ht/code/dbxfs
 Author: Rian Hunter
 Author-email: rian@alum.mit.edu
 License: GPL3
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3
@@ -53,15 +53,15 @@
 `fuse`.
 
 Run the following command:
 
     $ pip3 install dbxfs
 
 On Arch Linux and derivatives, you can find it in the AUR as
-[dbxfs](https://aur.archlinux.org/packages/dbxfs>).
+[dbxfs](https://aur.archlinux.org/packages/dbxfs).
 
 Usage
 -----
 
 Use `dbxfs` like you would use the `mount` command:
 
     $ dbxfs <mount_point>
```

### Comparing `dbxfs-2.0.0/setup.py` & `dbxfs-2.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 from setuptools import setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="dbxfs",
-    version='2.0.0',
+    version='2.0.1',
     author="Rian Hunter",
     author_email="rian@alum.mit.edu",
     description="User-space file system for Dropbox",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://thelig.ht/code/dbxfs',
     license="GPL3",
@@ -41,15 +41,15 @@
     install_requires=[
         # dropbox changes so often that we
         # just put a lower bound to avoid
         # dbxfs being uninstallable in the future
         # if dropbox=11 goes away.
         "dropbox>=11.25.0",
         "platformdirs>=4.1.0,<5",
-        "userspacefs>=3.0.0,<4",
+        "userspacefs>=3.1.0,<4",
         "block_tracing>=1.0.1,<2",
         "privy>=6.0,<7",
         "sentry_sdk>=1.39,<2",
         'pywin32;sys_platform=="win32"',
     ],
     extras_require={
         'safefs': ["safefs"],
```

