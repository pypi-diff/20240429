# Comparing `tmp/rssbot-553.tar.gz` & `tmp/rssbot-555.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rssbot-553.tar", last modified: Thu Apr 18 23:14:01 2024, max compression
+gzip compressed data, was "rssbot-555.tar", last modified: Mon Apr 29 11:14:20 2024, max compression
```

## Comparing `rssbot-553.tar` & `rssbot-555.tar`

### file list

```diff
@@ -1,36 +1,40 @@
-drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2024-04-18 23:14:01.655484 rssbot-553/
--rw-r--r--   0 bart      (1000) bart      (1000)     2322 2024-04-18 23:14:01.655484 rssbot-553/PKG-INFO
--rw-r--r--   0 bart      (1000) bart      (1000)     1785 2024-04-18 23:11:12.000000 rssbot-553/README.rst
-drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2024-04-18 23:14:01.655484 rssbot-553/bin/
--rwxr-xr-x   0 bart      (1000) bart      (1000)     4179 2024-04-18 23:11:12.000000 rssbot-553/bin/rssbot
--rwxr-xr-x   0 bart      (1000) bart      (1000)     2400 2024-04-18 23:11:12.000000 rssbot-553/bin/rssbotd
--rw-r--r--   0 bart      (1000) bart      (1000)      861 2024-04-18 23:11:12.000000 rssbot-553/pyproject.toml
-drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2024-04-18 23:14:01.655484 rssbot-553/rssbot/
--rw-r--r--   0 bart      (1000) bart      (1000)      876 2024-04-18 23:11:12.000000 rssbot-553/rssbot/__init__.py
--rw-r--r--   0 bart      (1000) bart      (1000)     1364 2024-04-18 23:11:12.000000 rssbot-553/rssbot/broker.py
--rw-r--r--   0 bart      (1000) bart      (1000)     3873 2024-04-18 23:11:12.000000 rssbot-553/rssbot/client.py
--rw-r--r--   0 bart      (1000) bart      (1000)     1922 2024-04-18 23:11:12.000000 rssbot-553/rssbot/command.py
--rw-r--r--   0 bart      (1000) bart      (1000)      230 2024-04-18 23:11:12.000000 rssbot-553/rssbot/default.py
--rw-r--r--   0 bart      (1000) bart      (1000)     1089 2024-04-18 23:11:12.000000 rssbot-553/rssbot/errors.py
--rw-r--r--   0 bart      (1000) bart      (1000)      766 2024-04-18 23:11:12.000000 rssbot-553/rssbot/event.py
--rw-r--r--   0 bart      (1000) bart      (1000)     1930 2024-04-18 23:11:12.000000 rssbot-553/rssbot/find.py
--rw-r--r--   0 bart      (1000) bart      (1000)     1362 2024-04-18 23:11:12.000000 rssbot-553/rssbot/handler.py
-drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2024-04-18 23:14:01.655484 rssbot-553/rssbot/modules/
--rw-r--r--   0 bart      (1000) bart      (1000)      231 2024-04-18 23:11:12.000000 rssbot-553/rssbot/modules/__init__.py
--rw-r--r--   0 bart      (1000) bart      (1000)      211 2024-04-18 23:11:12.000000 rssbot-553/rssbot/modules/cmd.py
--rw-r--r--   0 bart      (1000) bart      (1000)    17622 2024-04-18 23:11:12.000000 rssbot-553/rssbot/modules/irc.py
--rw-r--r--   0 bart      (1000) bart      (1000)    11001 2024-04-18 23:11:12.000000 rssbot-553/rssbot/modules/rss.py
--rw-r--r--   0 bart      (1000) bart      (1000)     6155 2024-04-18 23:11:12.000000 rssbot-553/rssbot/object.py
--rw-r--r--   0 bart      (1000) bart      (1000)      752 2024-04-18 23:11:12.000000 rssbot-553/rssbot/persist.py
--rw-r--r--   0 bart      (1000) bart      (1000)      275 2024-04-18 23:11:12.000000 rssbot-553/rssbot/repeater.py
--rw-r--r--   0 bart      (1000) bart      (1000)      109 2024-04-18 23:11:12.000000 rssbot-553/rssbot/runtime.py
--rw-r--r--   0 bart      (1000) bart      (1000)     1900 2024-04-18 23:11:12.000000 rssbot-553/rssbot/thread.py
--rw-r--r--   0 bart      (1000) bart      (1000)     1091 2024-04-18 23:11:12.000000 rssbot-553/rssbot/timer.py
--rw-r--r--   0 bart      (1000) bart      (1000)     1101 2024-04-18 23:11:12.000000 rssbot-553/rssbot/workdir.py
-drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2024-04-18 23:14:01.655484 rssbot-553/rssbot.egg-info/
--rw-r--r--   0 bart      (1000) bart      (1000)     2322 2024-04-18 23:14:01.000000 rssbot-553/rssbot.egg-info/PKG-INFO
--rw-r--r--   0 bart      (1000) bart      (1000)      548 2024-04-18 23:14:01.000000 rssbot-553/rssbot.egg-info/SOURCES.txt
--rw-r--r--   0 bart      (1000) bart      (1000)        1 2024-04-18 23:14:01.000000 rssbot-553/rssbot.egg-info/dependency_links.txt
--rw-r--r--   0 bart      (1000) bart      (1000)        7 2024-04-18 23:14:01.000000 rssbot-553/rssbot.egg-info/top_level.txt
--rw-r--r--   0 bart      (1000) bart      (1000)       38 2024-04-18 23:14:01.655484 rssbot-553/setup.cfg
--rw-r--r--   0 bart      (1000) bart      (1000)      185 2024-04-18 23:11:12.000000 rssbot-553/setup.py
+drwxr-xr-x   0 bart      (1000) bart      (1001)        0 2024-04-29 11:14:20.312440 rssbot-555/
+-rw-r--r--   0 bart      (1000) bart      (1001)     2322 2024-04-29 11:14:20.312440 rssbot-555/PKG-INFO
+-rw-r--r--   0 bart      (1000) bart      (1001)     1785 2024-04-28 14:36:32.000000 rssbot-555/README.rst
+drwxr-xr-x   0 bart      (1000) bart      (1001)        0 2024-04-29 11:14:20.308441 rssbot-555/bin/
+-rwxr-xr-x   0 bart      (1000) bart      (1001)     1111 2024-04-29 10:43:37.000000 rssbot-555/bin/rssbot
+-rwxr-xr-x   0 bart      (1000) bart      (1001)     2069 2024-04-29 10:39:51.000000 rssbot-555/bin/rssbotd
+-rw-r--r--   0 bart      (1000) bart      (1001)      861 2024-04-28 14:45:08.000000 rssbot-555/pyproject.toml
+drwxr-xr-x   0 bart      (1000) bart      (1001)        0 2024-04-29 11:14:20.312440 rssbot-555/rssbot/
+-rw-r--r--   0 bart      (1000) bart      (1001)       53 2024-04-28 14:24:03.000000 rssbot-555/rssbot/__init__.py
+-rw-r--r--   0 bart      (1000) bart      (1001)      704 2024-04-28 14:24:03.000000 rssbot-555/rssbot/broker.py
+-rw-r--r--   0 bart      (1000) bart      (1001)     4002 2024-04-28 14:24:03.000000 rssbot-555/rssbot/client.py
+-rw-r--r--   0 bart      (1000) bart      (1001)      581 2024-04-28 14:24:03.000000 rssbot-555/rssbot/command.py
+-rw-r--r--   0 bart      (1000) bart      (1001)      285 2024-04-28 14:24:03.000000 rssbot-555/rssbot/default.py
+-rw-r--r--   0 bart      (1000) bart      (1001)     1397 2024-04-28 14:24:03.000000 rssbot-555/rssbot/errors.py
+-rw-r--r--   0 bart      (1000) bart      (1001)      813 2024-04-28 14:24:03.000000 rssbot-555/rssbot/event.py
+-rw-r--r--   0 bart      (1000) bart      (1001)     2008 2024-04-28 14:24:03.000000 rssbot-555/rssbot/find.py
+-rw-r--r--   0 bart      (1000) bart      (1001)     1405 2024-04-28 14:24:03.000000 rssbot-555/rssbot/handler.py
+drwxr-xr-x   0 bart      (1000) bart      (1001)        0 2024-04-29 11:14:20.312440 rssbot-555/rssbot/modules/
+-rw-r--r--   0 bart      (1000) bart      (1001)      238 2024-04-29 10:45:21.000000 rssbot-555/rssbot/modules/__init__.py
+-rw-r--r--   0 bart      (1000) bart      (1001)      216 2024-04-28 14:24:09.000000 rssbot-555/rssbot/modules/cmd.py
+-rw-r--r--   0 bart      (1000) bart      (1001)      344 2024-04-28 14:24:09.000000 rssbot-555/rssbot/modules/err.py
+-rw-r--r--   0 bart      (1000) bart      (1001)      372 2024-04-28 14:24:09.000000 rssbot-555/rssbot/modules/flt.py
+-rw-r--r--   0 bart      (1000) bart      (1001)    18838 2024-04-28 14:32:53.000000 rssbot-555/rssbot/modules/irc.py
+-rw-r--r--   0 bart      (1000) bart      (1001)      183 2024-04-29 10:45:08.000000 rssbot-555/rssbot/modules/mod.py
+-rw-r--r--   0 bart      (1000) bart      (1001)    10834 2024-04-28 14:24:09.000000 rssbot-555/rssbot/modules/rss.py
+-rw-r--r--   0 bart      (1000) bart      (1001)      988 2024-04-28 14:24:09.000000 rssbot-555/rssbot/modules/thr.py
+-rw-r--r--   0 bart      (1000) bart      (1001)     6085 2024-04-28 14:24:03.000000 rssbot-555/rssbot/object.py
+-rw-r--r--   0 bart      (1000) bart      (1001)      278 2024-04-28 14:24:03.000000 rssbot-555/rssbot/repeater.py
+-rw-r--r--   0 bart      (1000) bart      (1001)     1260 2024-04-29 10:42:53.000000 rssbot-555/rssbot/runtime.py
+-rw-r--r--   0 bart      (1000) bart      (1001)     1956 2024-04-28 14:24:03.000000 rssbot-555/rssbot/thread.py
+-rw-r--r--   0 bart      (1000) bart      (1001)     1085 2024-04-28 14:24:03.000000 rssbot-555/rssbot/timer.py
+-rw-r--r--   0 bart      (1000) bart      (1001)     1120 2024-04-28 14:24:03.000000 rssbot-555/rssbot/whitelist.py
+-rw-r--r--   0 bart      (1000) bart      (1001)     1266 2024-04-28 14:24:03.000000 rssbot-555/rssbot/workdir.py
+drwxr-xr-x   0 bart      (1000) bart      (1001)        0 2024-04-29 11:14:20.312440 rssbot-555/rssbot.egg-info/
+-rw-r--r--   0 bart      (1000) bart      (1001)     2322 2024-04-29 11:14:20.000000 rssbot-555/rssbot.egg-info/PKG-INFO
+-rw-r--r--   0 bart      (1000) bart      (1001)      638 2024-04-29 11:14:20.000000 rssbot-555/rssbot.egg-info/SOURCES.txt
+-rw-r--r--   0 bart      (1000) bart      (1001)        1 2024-04-29 11:14:20.000000 rssbot-555/rssbot.egg-info/dependency_links.txt
+-rw-r--r--   0 bart      (1000) bart      (1001)        7 2024-04-29 11:14:20.000000 rssbot-555/rssbot.egg-info/top_level.txt
+-rw-r--r--   0 bart      (1000) bart      (1001)       38 2024-04-29 11:14:20.312440 rssbot-555/setup.cfg
+-rw-r--r--   0 bart      (1000) bart      (1001)      185 2024-04-28 14:22:49.000000 rssbot-555/setup.py
```

### Comparing `rssbot-553/PKG-INFO` & `rssbot-555/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rssbot
-Version: 553
+Version: 555
 Summary: 24/7 feed fetcher
 Author-email: Bart Thate <bthate@dds.nl>
 License: Public Domain
 Project-URL: home, https://pypi.org/project/rssbot
 Project-URL: bugs, https://github.com/xobjectz/rssbot/issues
 Project-URL: source, https://github.com/xobjectz/rssbot
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `rssbot-553/README.rst` & `rssbot-555/README.rst`

 * *Files identical despite different names*

### Comparing `rssbot-553/bin/rssbotd` & `rssbot-555/bin/rssbotd`

 * *Files 14% similar despite different names*

```diff
@@ -1,100 +1,89 @@
 #!/usr/bin/env python3
 # This file is placed in the Public Domain.
-#
-# pylint: disable=C,R,W0105,W0201,W0212,W0613,E0401,E0402,E0611
-# ruff: noqa: E402
 
 
 "daemon"
 
 
 import getpass
 import os
 import pwd
-import readline # pylint: disable=W0611
 import sys
 import time
 
 
-from rssbot.client  import spl
-from rssbot.command import Command
+from rssbot.command import add
 from rssbot.default import Default
 from rssbot.errors  import enable, errors
 from rssbot.object  import cdir
+from rssbot.runtime import init, scan
 from rssbot.workdir import Workdir, skel
 
 
 Cfg             = Default()
-Cfg.mod         = "cmd,irc,mod,rss"
+Cfg.mod         = "cmd,irc,rss"
 Cfg.opts        = ""
+Cfg.version     = "555"
 Cfg.name        = "rssbot"
-Cfg.version     = "552"
-Cfg.wd          = os.path.expanduser(f"~/.{Cfg.name}")
-Cfg.pidfile     = os.path.join(Cfg.wd, f"{Cfg.name}.pid")
-Workdir.workdir = Cfg.wd
+Cfg.user        = getpass.getuser()
+Cfg.wdr         = os.path.expanduser(f"~/.{Cfg.name}")
+Cfg.pidfile     = os.path.join(Cfg.wdr, f"{Cfg.name}.pid")
 
 
-from rssbot import modules
+Workdir.workdir = Cfg.wdr
 
 
-def daemon(pidfile, verbose=False):
+from rssbot import modules # pylint: disable=C0413
+
+
+def daemon(ppidfile, verbose=False):
+    "run in the background."
+    # pylint: disable=W0212
     pid = os.fork()
     if pid != 0:
         os._exit(0)
     os.setsid()
-    pid2 = os.fork()
-    if pid2 != 0:
+    pid22 = os.fork()
+    if pid22 != 0:
         os._exit(0)
     if not verbose:
-        with open('/dev/null', 'r', encoding="utf-8") as sis:
-            os.dup2(sis.fileno(), sys.stdin.fileno())
-        with open('/dev/null', 'a+', encoding="utf-8") as sos:
-            os.dup2(sos.fileno(), sys.stdout.fileno())
-        with open('/dev/null', 'a+', encoding="utf-8") as ses:
-            os.dup2(ses.fileno(), sys.stderr.fileno())
+        with open('/dev/null', 'r', encoding="utf-8") as siss:
+            os.dup2(siss.fileno(), sys.stdin.fileno())
+        with open('/dev/null', 'a+', encoding="utf-8") as soss:
+            os.dup2(soss.fileno(), sys.stdout.fileno())
+        with open('/dev/null', 'a+', encoding="utf-8") as sess:
+            os.dup2(sess.fileno(), sys.stderr.fileno())
     os.umask(0)
     os.chdir("/")
-    if os.path.exists(pidfile):
-        os.unlink(pidfile)
-    cdir(os.path.dirname(pidfile))
-    with open(pidfile, "w", encoding="utf-8") as fds:
-        fds.write(str(os.getpid()))
-
-
-def init(pkg, modstr, disable=""):
-    mds = []
-    for modname in spl(modstr):
-        if modname in spl(disable):
-            continue
-        module = getattr(pkg, modname, None)
-        if not module:
-            continue
-        if "init" in dir(module):
-            module.init()
-            mds.append(module)
-    return mds
+    if os.path.exists(ppidfile):
+        os.unlink(ppidfile)
+    cdir(os.path.dirname(ppidfile))
+    with open(ppidfile, "w", encoding="utf-8") as fdss:
+        fdss.write(str(os.getpid()))
 
 
 def privileges(username):
+    "lower privileges."
     pwnam = pwd.getpwnam(username)
     os.setgid(pwnam.pw_gid)
     os.setuid(pwnam.pw_uid)
 
 
 def ver(event):
+    "show version."
     event.reply(f"{Cfg.name.upper()} {Cfg.version}")
 
 
 def main():
-    Command.add(ver)
+    "main"
+    add(ver)
     enable(print)
     skel()
-    Cfg.mod = "," + ",".join(modules.__dir__())
-    Cfg.user = getpass.getuser()
+    scan(modules, Cfg.mod)
     daemon(Cfg.pidfile, "-v" in sys.argv)
     privileges(Cfg.user)
     init(modules, Cfg.mod)
     while 1:
         time.sleep(1.0)
```

### Comparing `rssbot-553/pyproject.toml` & `rssbot-555/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 ]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "rssbot"
 description = "24/7 feed fetcher"
-version = "553"
+version = "555"
 authors = [
     {name = "Bart Thate",email = "bthate@dds.nl"},
 ]
 readme = "README.rst"
 license = {text="Public Domain"}
 classifiers = [ 
     'Development Status :: 3 - Alpha',
```

### Comparing `rssbot-553/rssbot/client.py` & `rssbot-555/rssbot/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,8 @@
 # This file is placed in the Public Domain.
-#
-# pylint: disable=C,R,W0105,W0718
 
 
 "client"
 
 
 from .command import Command
 from .default import Default
@@ -53,15 +51,15 @@
 def command(bot, evt):
     "check for and run a command."
     parse_cmd(evt)
     func = getattr(Command.cmds, evt.cmd, None)
     if func:
         try:
             func(evt)
-        except Exception as exc:
+        except Exception as exc: # pylint: disable=W0718
             later(exc)
     bot.show(evt)
     evt.ready()
 
 
 def laps(seconds, short=True):
     "show elapsed time."
@@ -160,7 +158,18 @@
 def spl(txt):
     "split comma separated string into a list."
     try:
         res = txt.split(',')
     except (TypeError, ValueError):
         res = txt
     return [x for x in res if x]
+
+
+def __dir__():
+    return (
+        'Client',
+        'cmnd',
+        'command',
+        'lapse',
+        'parse_cmd',
+        'spl'
+    )
```

### Comparing `rssbot-553/rssbot/event.py` & `rssbot-555/rssbot/event.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,22 +1,20 @@
 # This file is placed in the Public Domain.
-#
-# pylint: disable=C,R,W0105
 
 
 "event"
 
 
 import threading
 
 
 from .default import Default
 
 
-class Event(Default):
+class Event(Default): # pylint: disable=R0902
 
     "Event"
 
     def __init__(self):
         Default.__init__(self)
         self._thr    = None
         self._ready  = threading.Event()
@@ -36,7 +34,13 @@
 
     def wait(self):
         "wait for event to be ready."
         if self._thr:
             self._thr.join()
         self._ready.wait()
         return self.result
+
+
+def __dir__():
+    return (
+        'Event',
+    )
```

### Comparing `rssbot-553/rssbot/find.py` & `rssbot-555/rssbot/find.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 # This file is placed in the Public Domain.
-#
-# pylint: disable=C,R,W0105
 
 
 "locate"
 
 
 import os
 import time
 
 
-from .default import Default
-from .object  import fqn, search, update
-from .persist import long
-from .workdir import fetch, store, strip
+from .default   import Default
+from .object    import fqn, search, update
+from .whitelist import long
+from .workdir   import fetch, store, strip
 
 
 def fns(mtc=""):
     "show list of files."
     dname = ''
     pth = store(mtc)
     for rootdir, dirs, _files in os.walk(pth, topdown=False):
@@ -71,7 +69,16 @@
                    )
     res = None
     if result:
         inp = result[-1]
         update(obj, inp[-1])
         res = inp[0]
     return res
+
+
+def __dir__():
+    return (
+        'fns',
+        'fntime',
+        'find',
+        'last'
+    )
```

### Comparing `rssbot-553/rssbot/handler.py` & `rssbot-555/rssbot/handler.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,8 @@
 # This file is placed in the Public Domain.
-#
-# pylint: disable=C,R,W0105,W0212
 
 
 "handler"
 
 
 import queue
 import threading
@@ -27,15 +25,15 @@
 
     def callback(self, evt):
         "call callback based on event type."
         func = getattr(self.cbs, evt.type, None)
         if not func:
             evt.ready()
             return
-        evt._thr = launch(func, self, evt)
+        evt._thr = launch(func, self, evt) # pylint: disable=W0212
 
     def loop(self):
         "proces events until interrupted."
         while not self.stopped.is_set():
             try:
                 evt = self.poll()
                 self.callback(evt)
@@ -57,7 +55,13 @@
     def start(self):
         "start the event loop."
         launch(self.loop)
 
     def stop(self):
         "stop the event loop."
         self.stopped.set()
+
+
+def __dir__():
+    return (
+        'Handler',
+    )
```

### Comparing `rssbot-553/rssbot/modules/irc.py` & `rssbot-555/rssbot/modules/irc.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,8 @@
 # This file is placed in the Public Domain.
-#
-# pylint: disable=C,R,W0105,W0612,W0718,E0402,W0201,W0603
-# ruff: noqa: F841
 
 
 "internet relay chat"
 
 
 import base64
 import os
@@ -14,60 +11,56 @@
 import ssl
 import textwrap
 import threading
 import time
 import _thread
 
 
-from ..client  import Client, command
-from ..command import Command
-from ..default import Default
-from ..errors  import debug, later
-from ..event   import Event
-from ..find    import last
-from ..object  import Object, edit, fmt, keys
-from ..persist import whitelist
-from ..runtime import broker
-from ..thread  import launch
-from ..workdir import sync
-
-
-NAME       = __file__.split(os.sep)[-3]
-filterlist = ["PING", "PONG", "PRIVMSG"]
-saylock    = _thread.allocate_lock()
-
-
-myirc = None
-
-
-def dbg(txt):
-    for flt in filterlist:
-        if flt in txt:
-            return
-    debug(txt)
+from ..client    import Client, command
+from ..default   import Default
+from ..event     import Event
+from ..errors    import Errors, debug, later
+from ..find      import last
+from ..object    import Object, edit, fmt, keys, values
+from ..runtime   import broker
+from ..thread    import launch
+from ..whitelist import whitelist
+from ..workdir   import sync
+
+
+NAME    = __file__.split(os.sep)[-3]
+saylock = _thread.allocate_lock()
+
+
+Errors.filter = ["PING", "PONG", "PRIVMSG"]
+
 
 def init():
-    global myirc
+    "initialize a irc bot."
     irc = IRC()
     irc.start()
     irc.events.joined.wait()
-    myirc = irc
     return irc
 
 
 def shutdown():
-    dbg(f"IRC stopping {myirc}")
-    if myirc:
-        myirc.state.pongcheck = True
-        myirc.state.keeprunning = False
-        myirc.events.connected.clear()
-        myirc.stop()
+    "shutdown irc bot."
+    for bot in values(broker.objs):
+        if "irc" not in str(type(bot)).lower():
+            continue
+        debug(f"IRC stopping {repr(bot)}")
+        bot.state.pongcheck = True
+        bot.state.keeprunning = False
+        bot.events.connected.clear()
+        bot.stop()
+
 
+class Config(Default): # pylint: disable=R0902,R0903
 
-class Config(Default):
+    "Config"
 
     channel = f'#{NAME}'
     commands = False
     control = '!'
     edited = time.time()
     nick = NAME
     port = 6667
@@ -92,14 +85,16 @@
 
 
 whitelist(Config)
 
 
 class TextWrap(textwrap.TextWrapper):
 
+    "TextWrap"
+
     def __init__(self):
         super().__init__()
         self.break_long_words = False
         self.drop_whitespace = False
         self.fix_sentence_endings = True
         self.replace_whitespace = True
         self.tabsize = 4
@@ -107,47 +102,54 @@
 
 
 wrapper = TextWrap()
 
 
 class Output():
 
+    "Output"
+
     cache = Object()
 
     def __init__(self):
         self.dostop = threading.Event()
         self.oqueue = queue.Queue()
 
     def dosay(self, channel, txt):
+        "overload this."
         raise NotImplementedError
 
     @staticmethod
     def extend(channel, txtlist):
+        "add list of txt to channel cache."
         if channel not in Output.cache:
             Output.cache[channel] = []
         chanlist = getattr(Output.cache, channel)
         chanlist.extend(txtlist)
 
     @staticmethod
     def gettxt(channel):
+        "return text from channel cache."
         txt = None
         try:
             che = getattr(Output.cache, channel, None)
             if che:
                 txt = che.pop(0)
         except (KeyError, IndexError):
             pass
         return txt
 
     def oput(self, channel, txt):
+        "put text to output queue."
         if channel and channel not in dir(Output.cache):
             setattr(Output.cache, channel, [])
         self.oqueue.put_nowait((channel, txt))
 
     def out(self):
+        "output loop."
         while not self.dostop.is_set():
             (channel, txt) = self.oqueue.get()
             if channel is None and txt is None:
                 break
             if self.dostop.is_set():
                 break
             txtlist = wrapper.wrap(txt)
@@ -162,21 +164,24 @@
             _nr = -1
             for txt in txtlist:
                 _nr += 1
                 self.dosay(channel, txt)
 
     @staticmethod
     def size(chan):
+        "return size of channel cache."
         if chan in Output.cache:
             return len(getattr(Output.cache, chan, []))
         return 0
 
 
 class IRC(Client, Output):
 
+    "IRC"
+
     def __init__(self):
         Client.__init__(self)
         Output.__init__(self)
         self.buffer = []
         self.cfg = Config()
         self.channels = []
         self.events = Default()
@@ -202,18 +207,20 @@
         self.register('NOTICE', cb_notice)
         self.register('PRIVMSG', cb_privmsg)
         self.register('QUIT', cb_quit)
         self.register("366", cb_ready)
         broker.add(self)
 
     def announce(self, txt):
+        "announce on all channels."
         for channel in self.channels:
             self.oput(channel, txt)
 
     def docommand(self, cmd, *args):
+        "send command to server."
         with saylock:
             if not args:
                 self.raw(cmd)
             elif len(args) == 1:
                 self.raw(f'{cmd.upper()} {args[0]}')
             elif len(args) == 2:
                 txt = ' '.join(args[1:])
@@ -222,18 +229,19 @@
                 txt = ' '.join(args[2:])
                 self.raw("{cmd.upper()} {args[0]} {args[1]} :{txt}")
             if (time.time() - self.state.last) < 5.0:
                 time.sleep(5.0)
             self.state.last = time.time()
 
     def connect(self, server, port=6667):
+        "connect to server."
         self.state.nrconnect += 1
         self.events.connected.clear()
         if self.cfg.password:
-            dbg("using SASL")
+            debug("using SASL")
             self.cfg.sasl = True
             self.cfg.port = "6697"
             ctx = ssl.SSLContext(ssl.PROTOCOL_TLS)
             ctx.options |= ssl.OP_NO_TLSv1 | ssl.OP_NO_TLSv1_1
             ctx.minimum_version = ssl.TLSVersion.TLSv1_2
             sock = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
             self.sock = ctx.wrap_socket(sock)
@@ -248,47 +256,51 @@
             self.sock.setblocking(True)
             self.sock.settimeout(180.0)
             self.events.connected.set()
             return True
         return False
 
     def direct(self, txt):
+        "send text directly on the socket."
         with saylock:
             self.raw(txt)
             time.sleep(2.0)
 
     def disconnect(self):
+        "disconnect from server."
         try:
             self.sock.shutdown(2)
         except (
                 ssl.SSLError,
                 OSError,
                 BrokenPipeError
-               ) as ex:
+               ) as _ex:
             pass
-        except Exception as ex:
+        except Exception as ex: # pylint: disable=W0718
             later(ex)
 
     def doconnect(self, server, nck, port=6667):
+        "loop until connected."
         while 1:
             try:
                 if self.connect(server, port):
                     break
             except (
                     ssl.SSLError,
                     OSError,
                     ConnectionResetError
                    ) as ex:
                 self.state.error = str(ex)
-                dbg(str(ex))
-            dbg(f"sleeping {self.cfg.sleep} seconds")
+                debug(str(ex))
+            debug(f"sleeping {self.cfg.sleep} seconds")
             time.sleep(self.cfg.sleep)
         self.logon(server, nck)
 
     def event(self, txt):
+        "create an event."
         evt = self.parsing(txt)
         cmd = evt.command
         if cmd == 'PING':
             self.state.pongcheck = True
             self.docommand('PONG', evt.txt or '')
         elif cmd == 'PONG':
             self.state.pongcheck = False
@@ -307,49 +319,54 @@
         elif cmd == '433':
             self.state.error = txt
             nck = self.cfg.nick + '_'
             self.docommand('NICK', nck)
         return evt
 
     def joinall(self):
+        "join all channels."
         for channel in self.channels:
             self.docommand('JOIN', channel)
 
     def keep(self):
+        "keep alive."
         while not self.stopped.is_set():
             if self.state.stopkeep:
                 self.state.stopkeep = False
                 break
             self.events.connected.wait()
             self.events.authed.wait()
             self.state.keeprunning = True
             time.sleep(self.cfg.sleep)
             self.state.pongcheck = True
             self.docommand('PING', self.cfg.server)
             if self.state.pongcheck:
-                dbg("failed pongcheck, restarting")
+                debug("failed pongcheck, restarting")
                 self.state.pongcheck = False
                 self.state.keeprunning = False
                 self.events.connected.clear()
                 self.stop()
                 init()
                 break
 
     def logon(self, server, nck):
+        "log onto server,"
         self.events.connected.wait()
         self.events.authed.wait()
         self.direct(f'NICK {nck}')
         self.direct(f'USER {nck} {server} {server} {nck}')
 
 
     def parsing(self, txt):
+        "parse text into an event."
+        # pylint: disable=R0912,R0915
         rawstr = str(txt)
         rawstr = rawstr.replace('\u0001', '')
         rawstr = rawstr.replace('\001', '')
-        dbg(txt)
+        debug(txt)
         obj = Event()
         obj.args = []
         obj.rawstr = rawstr
         obj.command = ''
         obj.arguments = []
         arguments = rawstr.split()
         if arguments:
@@ -399,14 +416,15 @@
             obj.rest = " ".join(obj.args)
         obj.orig = object.__repr__(self)
         obj.txt = obj.txt.strip()
         obj.type = obj.command
         return obj
 
     def poll(self):
+        "poll for event."
         self.events.connected.wait()
         if not self.buffer:
             try:
                 self.some()
             except BlockingIOError as ex:
                 time.sleep(1.0)
                 return self.event(str(ex))
@@ -416,26 +434,27 @@
                     ssl.SSLError,
                     ssl.SSLZeroReturnError,
                     ConnectionResetError,
                     BrokenPipeError
                    ) as ex:
                 later(ex)
                 self.stop()
-                dbg("handler stopped")
+                debug("handler stopped")
                 evt = self.event(str(ex))
                 return evt
         try:
             txt = self.buffer.pop(0)
         except IndexError:
             txt = ""
         return self.event(txt)
 
     def raw(self, txt):
+        "send raw text."
         txt = txt.rstrip()
-        dbg(txt)
+        debug(txt)
         txt = txt[:500]
         txt += '\r\n'
         txt = bytes(txt, 'utf-8')
         if self.sock:
             try:
                 self.sock.send(txt)
             except (
@@ -448,47 +467,52 @@
                 later(ex)
                 self.stop()
                 return
         self.state.last = time.time()
         self.state.nrsend += 1
 
     def reconnect(self):
-        dbg(f"reconnecting to {self.cfg.server}")
+        "reconnect to server."
+        debug(f"reconnecting to {self.cfg.server}")
         try:
             self.disconnect()
         except (ssl.SSLError, OSError):
             pass
         self.events.connected.clear()
         self.events.joined.clear()
         self.doconnect(self.cfg.server, self.cfg.nick, int(self.cfg.port))
 
     def dosay(self, channel, txt):
+        "method for output cache."
         self.events.joined.wait()
         txt = str(txt).replace('\n', '')
         txt = txt.replace('  ', ' ')
         self.docommand('PRIVMSG', channel, txt)
 
     def say(self, channel, txt):
+        "say text on channel."
         self.oput(channel, txt)
 
     def some(self):
+        "parse part of input text."
         self.events.connected.wait()
         if not self.sock:
             return
         inbytes = self.sock.recv(512)
         txt = str(inbytes, 'utf-8')
         if txt == '':
             raise ConnectionResetError
         self.state.lastline += txt
         splitted = self.state.lastline.split('\r\n')
         for line in splitted[:-1]:
             self.buffer.append(line)
         self.state.lastline = splitted[-1]
 
     def start(self):
+        "start bot."
         last(self.cfg)
         if self.cfg.channel not in self.channels:
             self.channels.append(self.cfg.channel)
         self.events.connected.clear()
         self.events.joined.clear()
         launch(Output.out, self)
         launch(Client.start, self)
@@ -498,101 +522,111 @@
                self.cfg.nick,
                int(self.cfg.port or '6667')
               )
         if not self.state.keeprunning:
             launch(self.keep)
 
     def stop(self):
+        "stop bot."
         self.state.stopkeep = True
         self.disconnect()
         self.dostop.set()
         self.oput(None, None)
         Client.stop(self)
 
     def wait(self):
+        "wait for ready."
         self.events.ready.wait()
 
 
 def cb_auth(bot, evt):
+    "auth callback."
     bot.docommand(f'AUTHENTICATE {bot.cfg.password}')
 
 
 def cb_cap(bot, evt):
+    "capabilities callback."
     if bot.cfg.password and 'ACK' in evt.arguments:
         bot.direct('AUTHENTICATE PLAIN')
     else:
         bot.direct('CAP REQ :sasl')
 
 
 def cb_error(bot, evt):
+    "error callback."
     if not bot.state.nrerror:
         bot.state.nrerror = 0
     bot.state.nrerror += 1
     bot.state.error = evt.txt
-    dbg(evt.txt)
+    debug(evt.txt)
 
 
 def cb_h903(bot, evt):
+    "auth succeded callback."
     bot.direct('CAP END')
     bot.events.authed.set()
 
 
 def cb_h904(bot, evt):
+    "auth succeded callback."
     bot.direct('CAP END')
     bot.events.authed.set()
 
 
 def cb_kill(bot, evt):
-    pass
+    "got killed callback."
 
 
 def cb_log(bot, evt):
-    pass
+    "log callback."
 
 
 def cb_ready(bot, evt):
+    "bot is ready callback."
     bot.events.ready.set()
 
 
 def cb_001(bot, evt):
+    "first line received callback."
     bot.logon()
 
 
 def cb_notice(bot, evt):
+    "notice callback."
     if evt.txt.startswith('VERSION'):
         txt = f'\001VERSION {NAME.upper()} 140 - {bot.cfg.username}\001'
         bot.docommand('NOTICE', evt.channel, txt)
 
 
 def cb_privmsg(bot, evt):
+    "privmsg callback."
     if not bot.cfg.commands:
         return
     if evt.txt:
         if evt.txt[0] in ['!',]:
             evt.txt = evt.txt[1:]
         elif evt.txt.startswith(f'{bot.cfg.nick}:'):
             evt.txt = evt.txt[len(bot.cfg.nick)+1:]
         else:
             return
         if evt.txt:
             evt.txt = evt.txt[0].lower() + evt.txt[1:]
-        dbg(f"command from {evt.origin}: {evt.txt}")
+        debug(f"command from {evt.origin}: {evt.txt}")
         command(bot, evt)
 
 
 def cb_quit(bot, evt):
-    dbg(f"quit from {bot.cfg.server}")
+    "quit callback."
+    debug(f"quit from {bot.cfg.server}")
     if evt.orig and evt.orig in bot.zelf:
         bot.stop()
 
 
-"commands"
-
-
 def cfg(event):
+    "configure command."
     config = Config()
     path = last(config)
     if not event.sets:
         event.reply(
                     fmt(
                         config,
                         keys(config),
@@ -601,18 +635,16 @@
                    )
     else:
         edit(config, event.sets)
         sync(config, path)
         event.reply('ok')
 
 
-Command.add(cfg)
-
-
 def mre(event):
+    "show from output cache."
     if not event.channel:
         event.reply('channel is not set.')
         return
     bot = broker.get(event.orig)
     if 'cache' not in dir(bot):
         event.reply('bot is missing cache')
         return
@@ -623,24 +655,19 @@
         txt = bot.gettxt(event.channel)
         if txt:
             bot.say(event.channel, txt)
     size = bot.size(event.channel)
     event.reply(f'{size} more in cache')
 
 
-Command.add(mre)
-
-
 def pwd(event):
+    "create a base64 password."
     if len(event.args) != 2:
         event.reply('pwd <nick> <password>')
         return
     arg1 = event.args[0]
     arg2 = event.args[1]
     txt = f'\x00{arg1}\x00{arg2}'
     enc = txt.encode('ascii')
     base = base64.b64encode(enc)
     dcd = base.decode('ascii')
     event.reply(dcd)
-
-
-Command.add(pwd)
```

### Comparing `rssbot-553/rssbot/modules/rss.py` & `rssbot-555/rssbot/modules/rss.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,8 @@
 # This file is placed in the Public Domain.
-#
-# pylint: disable=C,R,W0105
 
 
 "rich site syndicate"
 
 
 import html.parser
 import re
@@ -14,24 +12,22 @@
 import _thread
 
 
 from urllib.error import HTTPError, URLError
 from urllib.parse import quote_plus, urlencode
 
 
-from ..client   import laps, spl
-from ..command  import Command
-from ..default  import Default
-from ..find     import find, fntime, last
-from ..object   import Object, fmt, update, values
-from ..persist  import whitelist
-from ..repeater import Repeater
-from ..runtime  import broker
-from ..thread   import launch
-from ..workdir  import sync
+from ..client     import laps, spl
+from ..default    import Default
+from ..find       import find, fntime, last
+from ..object     import Object, fmt, update, values
+from ..repeater   import Repeater
+from ..runtime    import broker
+from ..thread     import launch
+from ..workdir    import sync
 
 
 def init():
     "start fetcher."
     fetcher = Fetcher()
     fetcher.start()
     return fetcher
@@ -47,30 +43,30 @@
     <head>
         <title>rssbot opml</title>
     </head>
     <body>
         <outline title="rssbot opml" text="24/7 feed fetcher">"""
 
 
-class Feed(Default):
+class Feed(Default): # pylint: disable=R0903
 
     "Feed"
 
 
-class Rss(Default):
+class Rss(Default): # pylint: disable=R0903
 
     "Rss"
 
     def __init__(self):
         Default.__init__(self)
         self.display_list = 'title,link,author'
         self.rss          = ''
 
 
-class Seen(Default):
+class Seen(Default): # pylint: disable=R0903
 
     "Seen"
 
     def __init__(self):
         Default.__init__(self)
         self.urls = []
 
@@ -320,17 +316,14 @@
 
 
 def useragent(txt):
     "return useragent."
     return 'Mozilla/5.0 (X11; Linux x86_64) ' + txt
 
 
-"commands"
-
-
 def dpl(event):
     "set display items."
     if len(event.args) < 2:
         event.reply('dpl <stringinurl> <item1,item2>')
         return
     setter = {'display_list': event.args[1]}
     for _fn, feed in find('rss', {'rss': event.args[0]}):
@@ -413,20 +406,7 @@
         if result:
             event.reply(f'already got {url}')
             return
     feed = Rss()
     feed.rss = event.args[0]
     sync(feed)
     event.reply('ok')
-
-
-"register"
-
-
-Command.add(dpl)
-Command.add(exp)
-Command.add(nme)
-Command.add(rem)
-Command.add(res)
-Command.add(rss)
-whitelist(Rss)
-whitelist(Seen)
```

### Comparing `rssbot-553/rssbot/object.py` & `rssbot-555/rssbot/object.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,20 @@
 # This file is placed in the Public Domain.
-#
-# pylint: disable=C,R,W0105
 
 
-"objects"
+"clean namespace"
 
 
 import json
 import os
 import pathlib
 import _thread
 
 
-disklock = _thread.allocate_lock()
+lock = _thread.allocate_lock()
 
 
 class Object:
 
     "Object"
 
     def __contains__(self, key):
@@ -113,15 +111,15 @@
     if isinstance(obj, type({})):
         return obj.keys()
     return list(obj.__dict__.keys())
 
 
 def read(obj, pth):
     "read an object from file path."
-    with disklock:
+    with lock:
         with open(pth, 'r', encoding='utf-8') as ofile:
             update(obj, load(ofile))
 
 
 def search(obj, selector):
     "check if object matches provided values."
     res = False
@@ -148,15 +146,15 @@
 def values(obj):
     "return values of an object."
     return obj.__dict__.values()
 
 
 def write(obj, pth):
     "write an object to disk."
-    with disklock:
+    with lock:
         cdir(os.path.dirname(pth))
         with open(pth, 'w', encoding='utf-8') as ofile:
             dump(obj, ofile, indent=4)
 
 
 class ObjectDecoder(json.JSONDecoder):
 
@@ -248,17 +246,14 @@
     "create directory."
     if os.path.exists(pth):
         return
     pth = pathlib.Path(pth)
     os.makedirs(pth, exist_ok=True)
 
 
-"interface"
-
-
 def __dir__():
     return (
         'Object',
         'construct',
         'dump',
         'dumps',
         'edit',
@@ -271,10 +266,7 @@
         'loads',
         'read',
         'search',
         'update',
         'values',
         'write'
     )
-
-
-__all__ = __dir__()
```

### Comparing `rssbot-553/rssbot/persist.py` & `rssbot-555/rssbot/whitelist.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,39 +1,58 @@
 # This file is placed in the Public Domain.
-#
-# pylint: disable=C,R,W0105
 
 
 "persist"
 
 
+import inspect
+
+
 from .object  import Object
 from .workdir import liststore
 
 
-class Persist(Object):
+class Whitelist(Object): # pylint: disable=R0903
 
-    "Persist"
+    "Whitelist"
 
     classes = Object()
 
 
+def scan(mod) -> None:
+    "scan module for classes."
+    for key, clz in inspect.getmembers(mod, inspect.isclass):
+        if key.startswith("cb"):
+            continue
+        if not issubclass(clz, Object):
+            continue
+        whitelist(clz)
+
+
 def whitelist(clz):
     "add class to whitelist."
     name = str(clz).split()[1][1:-2]
-    setattr(Persist.classes, name, clz)
+    setattr(Whitelist.classes, name, clz)
 
 
 def long(name):
     "match from single name to long name."
     split = name.split(".")[-1].lower()
     res = name
-    for named in Persist.classes:
+    for named in Whitelist.classes:
         if split in named.split(".")[-1].lower():
             res = named
             break
     if "." not in res:
         for fnm in liststore():
             claz = fnm.split(".")[-1]
             if fnm == claz.lower():
                 res = fnm
     return res
+
+
+def __dir__():
+    return (
+        'Whitelist',
+        'long',
+        'whitelist'
+    )
```

### Comparing `rssbot-553/rssbot/thread.py` & `rssbot-555/rssbot/thread.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,8 @@
 # This file is placed in the Public Domain.
-#
-# pylint: disable=C,R,W0105,W0718
 
 
 "thread"
 
 
 import queue
 import threading
@@ -28,28 +26,27 @@
         self.starttime = time.time()
         self.queue.put_nowait((func, args))
 
     def __iter__(self):
         return self
 
     def __next__(self):
-        for k in dir(self):
-            yield k
+        yield from dir(self)
 
     def join(self, timeout=1.0):
         "join this thread."
         super().join(timeout)
         return self._result
 
     def run(self):
         "run this thread's payload."
         func, args = self.queue.get()
         try:
             self._result = func(*args)
-        except Exception as ex:
+        except Exception as ex: # pylint: disable=W0718
             later(ex)
             if args and "Event" in str(type(args[0])):
                 args[0].ready()
 
 
 def launch(func, *args, **kwargs):
     "launch a thread."
@@ -69,7 +66,15 @@
     if '__class__' in dir(obj) and '__name__' in dir(obj):
         return f'{obj.__class__.__name__}.{obj.__name__}'
     if '__class__' in dir(obj):
         return f"{obj.__class__.__module__}.{obj.__class__.__name__}"
     if '__name__' in dir(obj):
         return f'{obj.__class__.__name__}.{obj.__name__}'
     return None
+
+
+def __dir__():
+    return (
+        'Thread',
+        'launch',
+        'name'
+    )
```

### Comparing `rssbot-553/rssbot/timer.py` & `rssbot-555/rssbot/timer.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,25 +1,23 @@
 # This file is placed in the Public Domain.
-#
-# pylint: disable=C,R,W0105
 
 
 "timer"
 
 
 import threading
 import time
 
 
 from .thread import launch
 
 
 class Timer:
 
-    "run a function at a specific time."
+    "Timer"
 
     def __init__(self, sleep, func, *args, thrname=None):
         self.args  = args
         self.func  = func
         self.sleep = sleep
         self.name  = thrname or str(self.func).split()[2]
         self.state = {}
@@ -43,7 +41,13 @@
         timer.start()
         self.timer   = timer
 
     def stop(self):
         "stop timer."
         if self.timer:
             self.timer.cancel()
+
+
+def __dir__():
+    return (
+        'Timer',
+    )
```

### Comparing `rssbot-553/rssbot/workdir.py` & `rssbot-555/rssbot/workdir.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 # This file is placed in the Public Domain.
-#
-# pylint: disable=C,R
 
 
-"working directory"
+"workdir"
 
 
 import datetime
 import os
 
 
 from .object import Object, cdir, fqn, read, write
 
 
-class Workdir(Object):
+class Workdir(Object): # pylint: disable=R0903
 
     "Workdir"
 
     workdir = ""
 
 
 def fetch(obj, pth):
@@ -58,7 +56,20 @@
 def sync(obj, pth=None):
     "sync object to disk."
     if pth is None:
         pth = ident(obj)
     pth2 = store(pth)
     write(obj, pth2)
     return pth
+
+
+def __dir__():
+    return (
+        'Workdir',
+        'fetch',
+        'ident',
+        'liststore',
+        'skel',
+        'store',
+        'strip',
+        'sync'
+    )
```

### Comparing `rssbot-553/rssbot.egg-info/PKG-INFO` & `rssbot-555/rssbot.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rssbot
-Version: 553
+Version: 555
 Summary: 24/7 feed fetcher
 Author-email: Bart Thate <bthate@dds.nl>
 License: Public Domain
 Project-URL: home, https://pypi.org/project/rssbot
 Project-URL: bugs, https://github.com/xobjectz/rssbot/issues
 Project-URL: source, https://github.com/xobjectz/rssbot
 Classifier: Development Status :: 3 - Alpha
```

