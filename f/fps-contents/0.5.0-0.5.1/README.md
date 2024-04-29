# Comparing `tmp/fps_contents-0.5.0.tar.gz` & `tmp/fps_contents-0.5.1.tar.gz`

## Comparing `fps_contents-0.5.0.tar` & `fps_contents-0.5.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 fps_contents-0.5.0/MANIFEST.in
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 fps_contents-0.5.0/fps_contents/__init__.py
--rw-r--r--   0        0        0     8568 2020-02-02 00:00:00.000000 fps_contents-0.5.0/fps_contents/fileid.py
--rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 fps_contents-0.5.0/fps_contents/main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fps_contents-0.5.0/fps_contents/py.typed
--rw-r--r--   0        0        0    10064 2020-02-02 00:00:00.000000 fps_contents-0.5.0/fps_contents/routes.py
--rw-r--r--   0        0        0     6386 2020-02-02 00:00:00.000000 fps_contents-0.5.0/.gitignore
--rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 fps_contents-0.5.0/COPYING.md
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 fps_contents-0.5.0/README.md
--rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 fps_contents-0.5.0/pyproject.toml
--rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 fps_contents-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 fps_contents-0.5.1/MANIFEST.in
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 fps_contents-0.5.1/fps_contents/__init__.py
+-rw-r--r--   0        0        0     8736 2020-02-02 00:00:00.000000 fps_contents-0.5.1/fps_contents/fileid.py
+-rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 fps_contents-0.5.1/fps_contents/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fps_contents-0.5.1/fps_contents/py.typed
+-rw-r--r--   0        0        0    10064 2020-02-02 00:00:00.000000 fps_contents-0.5.1/fps_contents/routes.py
+-rw-r--r--   0        0        0     6386 2020-02-02 00:00:00.000000 fps_contents-0.5.1/.gitignore
+-rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 fps_contents-0.5.1/COPYING.md
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 fps_contents-0.5.1/README.md
+-rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 fps_contents-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 fps_contents-0.5.1/PKG-INFO
```

### Comparing `fps_contents-0.5.0/fps_contents/fileid.py` & `fps_contents-0.5.1/fps_contents/fileid.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,15 +5,17 @@
 
 import aiosqlite
 from anyio import Path
 from watchfiles import Change, awatch
 
 from jupyverse_api import Singleton
 
-logger = logging.getLogger("contents")
+contents_logger = logging.getLogger("contents")
+watchfiles_logger = logging.getLogger("watchfiles")
+watchfiles_logger.setLevel(logging.WARNING)
 
 
 class Watcher:
     def __init__(self, path: str) -> None:
         self.path = path
         self._event = asyncio.Event()
 
@@ -106,54 +108,54 @@
                     added_paths = set()
                     for change, changed_path in changes:
                         # get relative path
                         changed_path = Path(changed_path).relative_to(await Path().absolute())
                         changed_path_str = str(changed_path)
 
                         if change == Change.deleted:
-                            logger.debug("File %s was deleted", changed_path_str)
+                            contents_logger.debug("File %s was deleted", changed_path_str)
                             async with db.execute(
                                 "SELECT COUNT(*) FROM fileids WHERE path = ?", (changed_path_str,)
                             ) as cursor:
                                 if not (await cursor.fetchone())[0]:
                                     # path is not indexed, ignore
-                                    logger.debug(
+                                    contents_logger.debug(
                                         "File %s is not indexed, ignoring", changed_path_str
                                     )
                                     continue
                             # path is indexed
                             await maybe_rename(
                                 db, changed_path_str, deleted_paths, added_paths, False
                             )
                         elif change == Change.added:
-                            logger.debug("File %s was added", changed_path_str)
+                            contents_logger.debug("File %s was added", changed_path_str)
                             await maybe_rename(
                                 db, changed_path_str, added_paths, deleted_paths, True
                             )
                         elif change == Change.modified:
-                            logger.debug("File %s was modified", changed_path_str)
+                            contents_logger.debug("File %s was modified", changed_path_str)
                             if changed_path_str == self.db_path:
                                 continue
                             async with db.execute(
                                 "SELECT COUNT(*) FROM fileids WHERE path = ?", (changed_path_str,)
                             ) as cursor:
                                 if not (await cursor.fetchone())[0]:
                                     # path is not indexed, ignore
-                                    logger.debug(
+                                    contents_logger.debug(
                                         "File %s is not indexed, ignoring", changed_path_str
                                     )
                                     continue
                             mtime = (await changed_path.stat()).st_mtime
                             await db.execute(
                                 "UPDATE fileids SET mtime = ? WHERE path = ?",
                                 (mtime, changed_path_str),
                             )
 
                     for path in deleted_paths - added_paths:
-                        logger.debug("Unindexing file %s ", path)
+                        contents_logger.debug("Unindexing file %s ", path)
                         await db.execute("DELETE FROM fileids WHERE path = ?", (path,))
                     await db.commit()
 
             for change in changes:
                 changed_path = change[1]
                 # get relative path
                 relative_changed_path = str(Path(changed_path).relative_to(await Path().absolute()))
@@ -199,12 +201,12 @@
     for other_path in other_paths:
         mtime2 = await get_mtime(other_path, db_or_fs2)
         if mtime1 == mtime2:
             # same files, according to modification times
             path1, path2 = changed_path, other_path
             if is_added_path:
                 path1, path2 = path2, path1
-            logger.debug("File %s was renamed to %s", path1, path2)
+            contents_logger.debug("File %s was renamed to %s", path1, path2)
             await db.execute("UPDATE fileids SET path = ? WHERE path = ?", (path2, path1))
             other_paths.remove(other_path)
             return
     changed_paths.add(changed_path)
```

### Comparing `fps_contents-0.5.0/fps_contents/routes.py` & `fps_contents-0.5.1/fps_contents/routes.py`

 * *Files identical despite different names*

### Comparing `fps_contents-0.5.0/.gitignore` & `fps_contents-0.5.1/.gitignore`

 * *Files identical despite different names*

### Comparing `fps_contents-0.5.0/COPYING.md` & `fps_contents-0.5.1/COPYING.md`

 * *Files identical despite different names*

### Comparing `fps_contents-0.5.0/pyproject.toml` & `fps_contents-0.5.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fps_contents-0.5.0/PKG-INFO` & `fps_contents-0.5.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: fps_contents
-Version: 0.5.0
+Version: 0.5.1
 Summary: An FPS plugin for the contents API
 Project-URL: Homepage, https://jupyter.org
 Author-email: Jupyter Development Team <jupyter@googlegroups.com>
 License: BSD 3-Clause License
 License-File: COPYING.md
 Keywords: fastapi,jupyter,plugins,server
 Requires-Python: >=3.8
```

