# Comparing `tmp/project_harpy-0.0.10.tar.gz` & `tmp/project.harpy-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "project_harpy-0.0.10.tar", last modified: Mon Apr 29 04:35:30 2024, max compression
+gzip compressed data, was "project.harpy-0.0.9.tar", last modified: Mon Jan  8 08:28:34 2024, max compression
```

## Comparing `project_harpy-0.0.10.tar` & `project.harpy-0.0.9.tar`

### file list

```diff
@@ -1,24 +1,25 @@
-drwxr-xr-x   0 serhat    (1000) serhat    (1000)        0 2024-04-29 04:35:30.431293 project_harpy-0.0.10/
--rw-r--r--   0 serhat    (1000) serhat    (1000)     1070 2024-04-29 04:35:16.000000 project_harpy-0.0.10/LICENSE
--rw-r--r--   0 serhat    (1000) serhat    (1000)      769 2024-04-29 04:35:30.431293 project_harpy-0.0.10/PKG-INFO
-drwxr-xr-x   0 serhat    (1000) serhat    (1000)        0 2024-04-29 04:35:30.427960 project_harpy-0.0.10/harpy/
--rw-r--r--   0 serhat    (1000) serhat    (1000)        0 2024-04-29 04:35:16.000000 project_harpy-0.0.10/harpy/__init__.py
--rw-r--r--   0 serhat    (1000) serhat    (1000)     2200 2024-04-29 04:35:16.000000 project_harpy-0.0.10/harpy/__main__.py
--rw-r--r--   0 serhat    (1000) serhat    (1000)       79 2024-04-29 04:35:16.000000 project_harpy-0.0.10/harpy/__version__.py
--rw-r--r--   0 serhat    (1000) serhat    (1000)      495 2024-04-29 04:35:16.000000 project_harpy-0.0.10/harpy/argtypes.py
--rw-r--r--   0 serhat    (1000) serhat    (1000)     2456 2024-04-29 04:35:16.000000 project_harpy-0.0.10/harpy/cli.py
--rw-r--r--   0 serhat    (1000) serhat    (1000)      707 2024-04-29 04:35:16.000000 project_harpy-0.0.10/harpy/consts.py
--rw-r--r--   0 serhat    (1000) serhat    (1000)  1150157 2024-04-29 04:35:16.000000 project_harpy-0.0.10/harpy/db.json
--rw-r--r--   0 serhat    (1000) serhat    (1000)      572 2024-04-29 04:35:16.000000 project_harpy-0.0.10/harpy/globs.py
--rw-r--r--   0 serhat    (1000) serhat    (1000)     1218 2024-04-29 04:35:16.000000 project_harpy-0.0.10/harpy/handlers.py
--rw-r--r--   0 serhat    (1000) serhat    (1000)     5353 2024-04-29 04:35:16.000000 project_harpy-0.0.10/harpy/net.py
--rw-r--r--   0 serhat    (1000) serhat    (1000)     1512 2024-04-29 04:35:16.000000 project_harpy-0.0.10/harpy/utils.py
-drwxr-xr-x   0 serhat    (1000) serhat    (1000)        0 2024-04-29 04:35:30.427960 project_harpy-0.0.10/project.harpy.egg-info/
--rw-r--r--   0 serhat    (1000) serhat    (1000)      769 2024-04-29 04:35:30.000000 project_harpy-0.0.10/project.harpy.egg-info/PKG-INFO
--rw-r--r--   0 serhat    (1000) serhat    (1000)      425 2024-04-29 04:35:30.000000 project_harpy-0.0.10/project.harpy.egg-info/SOURCES.txt
--rw-r--r--   0 serhat    (1000) serhat    (1000)        1 2024-04-29 04:35:30.000000 project_harpy-0.0.10/project.harpy.egg-info/dependency_links.txt
--rw-r--r--   0 serhat    (1000) serhat    (1000)       46 2024-04-29 04:35:30.000000 project_harpy-0.0.10/project.harpy.egg-info/entry_points.txt
--rw-r--r--   0 serhat    (1000) serhat    (1000)        1 2024-04-29 04:35:29.000000 project_harpy-0.0.10/project.harpy.egg-info/not-zip-safe
--rw-r--r--   0 serhat    (1000) serhat    (1000)        6 2024-04-29 04:35:30.000000 project_harpy-0.0.10/project.harpy.egg-info/top_level.txt
--rw-r--r--   0 serhat    (1000) serhat    (1000)     1052 2024-04-29 04:35:16.000000 project_harpy-0.0.10/pyproject.toml
--rw-r--r--   0 serhat    (1000) serhat    (1000)       38 2024-04-29 04:35:30.431293 project_harpy-0.0.10/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-01-08 08:28:34.600769 project.harpy-0.0.9/
+-rw-rw-rw-   0        0        0     1091 2024-01-08 02:09:06.000000 project.harpy-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0      788 2024-01-08 08:28:34.597892 project.harpy-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0       60 2024-01-08 02:09:06.000000 project.harpy-0.0.9/README.md
+drwxrwxrwx   0        0        0        0 2024-01-08 08:28:34.570187 project.harpy-0.0.9/harpy/
+-rw-rw-rw-   0        0        0        0 2024-01-08 02:09:06.000000 project.harpy-0.0.9/harpy/__init__.py
+-rw-rw-rw-   0        0        0     2299 2024-01-08 02:09:06.000000 project.harpy-0.0.9/harpy/__main__.py
+-rw-rw-rw-   0        0        0       81 2024-01-08 08:27:14.000000 project.harpy-0.0.9/harpy/__version__.py
+-rw-rw-rw-   0        0        0      514 2024-01-08 02:09:06.000000 project.harpy-0.0.9/harpy/argtypes.py
+-rw-rw-rw-   0        0        0     2573 2024-01-08 02:09:06.000000 project.harpy-0.0.9/harpy/cli.py
+-rw-rw-rw-   0        0        0      745 2024-01-08 02:09:06.000000 project.harpy-0.0.9/harpy/consts.py
+-rw-rw-rw-   0        0        0  1150157 2024-01-08 02:09:06.000000 project.harpy-0.0.9/harpy/db.json
+-rw-rw-rw-   0        0        0      600 2024-01-08 02:09:06.000000 project.harpy-0.0.9/harpy/globs.py
+-rw-rw-rw-   0        0        0     1268 2024-01-08 08:25:35.000000 project.harpy-0.0.9/harpy/handlers.py
+-rw-rw-rw-   0        0        0     5543 2024-01-08 02:09:06.000000 project.harpy-0.0.9/harpy/net.py
+-rw-rw-rw-   0        0        0     1570 2024-01-08 02:09:06.000000 project.harpy-0.0.9/harpy/utils.py
+drwxrwxrwx   0        0        0        0 2024-01-08 08:28:34.597892 project.harpy-0.0.9/project.harpy.egg-info/
+-rw-rw-rw-   0        0        0      788 2024-01-08 08:28:34.000000 project.harpy-0.0.9/project.harpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      435 2024-01-08 08:28:34.000000 project.harpy-0.0.9/project.harpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-01-08 08:28:34.000000 project.harpy-0.0.9/project.harpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2024-01-08 08:28:34.000000 project.harpy-0.0.9/project.harpy.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2024-01-08 08:28:33.000000 project.harpy-0.0.9/project.harpy.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0        6 2024-01-08 08:28:34.000000 project.harpy-0.0.9/project.harpy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1089 2024-01-08 02:09:06.000000 project.harpy-0.0.9/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-01-08 08:28:34.600769 project.harpy-0.0.9/setup.cfg
```

### Comparing `project_harpy-0.0.10/PKG-INFO` & `project.harpy-0.0.9/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-Metadata-Version: 2.1
-Name: project.harpy
-Version: 0.0.10
-Summary: Active/passive ARP discovery tool
-Author: Serhat Çelik
-License: MIT
-Keywords: harpy,arp,discovery
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Environment :: Console
-Classifier: Intended Audience :: Information Technology
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Topic :: System :: Networking
-Classifier: Topic :: System :: Networking :: Monitoring
-Requires-Python: <3.12,>=3.9
-License-File: LICENSE
+Metadata-Version: 2.1
+Name: project.harpy
+Version: 0.0.9
+Summary: Active/passive ARP discovery tool
+Author: Serhat Çelik
+License: MIT
+Keywords: harpy,arp,discovery
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Environment :: Console
+Classifier: Intended Audience :: Information Technology
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: System :: Networking
+Classifier: Topic :: System :: Networking :: Monitoring
+Requires-Python: <3.12,>=3.9
+License-File: LICENSE
```

### Comparing `project_harpy-0.0.10/harpy/__main__.py` & `project.harpy-0.0.9/harpy/__main__.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,99 +1,99 @@
-"""hARPy — Active/passive ARP discovery tool."""
-
-import atexit
-import os
-import signal
-import socket
-import threading
-
-from harpy.cli import Namespace, parser
-from harpy.consts import (
-    CLS,
-    GGP,
-    LOGO,
-    PORT,
-    WAIT_PRINT,
-)
-from harpy.globs import controller, interrupts, sent
-from harpy.handlers import Echo, Is
-from harpy.net import Sender, Sniffer
-from harpy.utils import get_manuf_db, ignore, safesignal
-
-
-def start() -> list[threading.Thread]:
-    """Start the program."""
-    opts = parser.parse_args(namespace=Namespace())
-
-    safesignal(signal.SIGINT, stop)
-
-    Echo.disable()
-
-    sock = socket.socket(socket.PF_PACKET, socket.SOCK_RAW, socket.htons(GGP))
-
-    atexit.register(sock.close)
-
-    sock.setblocking(False)  # Non-blocking mode
-
-    sock.setsockopt(socket.SOL_SOCKET, socket.SO_REUSEADDR, 1)
-    sock.setsockopt(socket.SOL_SOCKET, socket.SO_REUSEPORT, 1)
-
-    sock.bind((opts.device, PORT))
-
-    db = get_manuf_db(os.path.join(os.path.dirname(__file__), 'db.json'))
-
-    threads = []  # type: list[threading.Thread]
-
-    network = opts.network
-
-    sniffer = Sniffer(sock, network, db, opts.F, opts.S)
-    threads.append(sniffer)
-
-    if not opts.p:
-        sender = Sender(sock, network, opts.node, opts.sleep, opts.f, opts.R)
-        threads.append(sender)
-
-    for thread in threads:
-        thread.start()
-
-    while not controller.wait(WAIT_PRINT):  # Non-blocking wait
-        with ignore(signal.SIGINT):
-            print(CLS, *LOGO, *sniffer, opts() + '>\t' + sent.get(), sep='\n')
-
-    return threads
-
-
-def stop(*args) -> None:
-    """Stop the program."""
-    safesignal(signal.SIGINT, signal.SIG_IGN)
-    controller.set()
-
-
-def join(threads: list[threading.Thread]) -> None:
-    """Join all threads."""
-    for thread in threads:
-        thread.join()
-
-
-def log() -> None:
-    """Print the interrupt messages, if any."""
-    for message in interrupts:
-        print(message)
-
-
-def main() -> None:
-    """Entry point."""
-    if not Is.atty():  # Order matters!
-        return
-    if not Is.fore():
-        return
-    if not Is.root():
-        parser.print_help()
-        return
-
-    join(start())
-
-    log()
-
-
-if __name__ == '__main__':
-    main()
+"""hARPy — Active/passive ARP discovery tool."""
+
+import atexit
+import os
+import signal
+import socket
+import threading
+
+from harpy.cli import Namespace, parser
+from harpy.consts import (
+    CLS,
+    GGP,
+    LOGO,
+    PORT,
+    WAIT_PRINT,
+)
+from harpy.globs import controller, interrupts, sent
+from harpy.handlers import Echo, Is
+from harpy.net import Sender, Sniffer
+from harpy.utils import get_manuf_db, ignore, safesignal
+
+
+def start() -> list[threading.Thread]:
+    """Start the program."""
+    opts = parser.parse_args(namespace=Namespace())
+
+    safesignal(signal.SIGINT, stop)
+
+    Echo.disable()
+
+    sock = socket.socket(socket.PF_PACKET, socket.SOCK_RAW, socket.htons(GGP))
+
+    atexit.register(sock.close)
+
+    sock.setblocking(False)  # Non-blocking mode
+
+    sock.setsockopt(socket.SOL_SOCKET, socket.SO_REUSEADDR, 1)
+    sock.setsockopt(socket.SOL_SOCKET, socket.SO_REUSEPORT, 1)
+
+    sock.bind((opts.device, PORT))
+
+    db = get_manuf_db(os.path.join(os.path.dirname(__file__), 'db.json'))
+
+    threads = []  # type: list[threading.Thread]
+
+    network = opts.network
+
+    sniffer = Sniffer(sock, network, db, opts.F, opts.S)
+    threads.append(sniffer)
+
+    if not opts.p:
+        sender = Sender(sock, network, opts.node, opts.sleep, opts.f, opts.R)
+        threads.append(sender)
+
+    for thread in threads:
+        thread.start()
+
+    while not controller.wait(WAIT_PRINT):  # Non-blocking wait
+        with ignore(signal.SIGINT):
+            print(CLS, *LOGO, *sniffer, opts() + '>\t' + sent.get(), sep='\n')
+
+    return threads
+
+
+def stop(*args) -> None:
+    """Stop the program."""
+    safesignal(signal.SIGINT, signal.SIG_IGN)
+    controller.set()
+
+
+def join(threads: list[threading.Thread]) -> None:
+    """Join all threads."""
+    for thread in threads:
+        thread.join()
+
+
+def log() -> None:
+    """Print the interrupt messages, if any."""
+    for message in interrupts:
+        print(message)
+
+
+def main() -> None:
+    """Entry point."""
+    if not Is.atty():  # Order matters!
+        return
+    if not Is.fore():
+        return
+    if not Is.root():
+        parser.print_help()
+        return
+
+    join(start())
+
+    log()
+
+
+if __name__ == '__main__':
+    main()
```

### Comparing `project_harpy-0.0.10/harpy/cli.py` & `project.harpy-0.0.9/harpy/cli.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,111 +1,111 @@
-"""Command-line interface."""
-
-import argparse
-
-from harpy.__version__ import __version__
-from harpy.argtypes import device, ipv4
-from harpy.consts import (
-    DEFAULT_OCTET,
-    DEFAULT_SLEEP,
-)
-from harpy.utils import get_devices
-
-
-class Namespace(argparse.Namespace):
-    """Simple object for storing attributes."""
-
-    def __call__(self) -> str:
-        """Get currently active modes."""
-        return ''.join(k for k, v in vars(self).items() if len(k) == 1 and v)
-
-
-parser = argparse.ArgumentParser(
-    prog='harpy',
-    description='%(prog)s — active/passive arp discovery tool',
-    epilog='https://github.com/x3525/harpy',
-    formatter_class=argparse.RawTextHelpFormatter,
-)
-
-modes = parser.add_argument_group('modes')
-
-mutual = modes.add_mutually_exclusive_group()
-
-###############
-# Positionals #
-###############
-parser.add_argument(
-    'network',
-    type=ipv4,
-    help='ip range in cidr format',
-    metavar='range',
-)
-
-###########
-# Options #
-###########
-parser.add_argument(
-    '-i',
-    default=next(iter(devices := get_devices()), ''),
-    type=device,
-    choices=devices,
-    help='use %(metavar)s as network device (default: %(default)s)',
-    metavar='DEVICE',
-    dest='device',
-)
-parser.add_argument(
-    '-n',
-    default=DEFAULT_OCTET,
-    type=int,
-    choices=range(2, 254),
-    help='use %(metavar)s as last ip octet for sending (default: %(default)s)',
-    metavar='NODE',
-    dest='node',
-)
-parser.add_argument(
-    '-s',
-    default=DEFAULT_SLEEP,
-    type=int,
-    help='sleep %(metavar)s ms between each request (default: %(default)s)',
-    metavar='TIME',
-    dest='sleep',
-)
-parser.add_argument(
-    '-v',
-    action='version',
-    help='show program version and exit',
-    version=__version__,
-)
-
-##################
-# Options: Modes #
-##################
-modes.add_argument(
-    '-f',
-    action='store_true',
-    help='enable fast mode, only scan specific hosts',
-    dest='f',
-)
-modes.add_argument(
-    '-F',
-    action='store_true',
-    help='enable filter mode, exclude hosts not in range',
-    dest='F',
-)
-mutual.add_argument(
-    '-p',
-    action='store_true',
-    help='enable passive mode, do not send any packets',
-    dest='p',
-)
-mutual.add_argument(
-    '-R',
-    action='store_true',
-    help='enable continuous mode, never stop sending packets',
-    dest='R',
-)
-modes.add_argument(
-    '-S',
-    action='store_true',
-    help='enable strict mode, treat inconsistent packets as new',
-    dest='S',
-)
+"""Command-line interface."""
+
+import argparse
+
+from harpy.__version__ import __version__
+from harpy.argtypes import device, ipv4
+from harpy.consts import (
+    DEFAULT_OCTET,
+    DEFAULT_SLEEP,
+)
+from harpy.utils import get_devices
+
+
+class Namespace(argparse.Namespace):
+    """Simple object for storing attributes."""
+
+    def __call__(self) -> str:
+        """Get currently active modes."""
+        return ''.join(k for k, v in vars(self).items() if len(k) == 1 and v)
+
+
+parser = argparse.ArgumentParser(
+    prog='harpy',
+    description='%(prog)s — active/passive arp discovery tool',
+    epilog='https://github.com/serhatcelik/harpy',
+    formatter_class=argparse.RawTextHelpFormatter,
+)
+
+modes = parser.add_argument_group('modes')
+
+mutual = modes.add_mutually_exclusive_group()
+
+###############
+# Positionals #
+###############
+parser.add_argument(
+    'network',
+    type=ipv4,
+    help='ip range in cidr format',
+    metavar='range',
+)
+
+###########
+# Options #
+###########
+parser.add_argument(
+    '-i',
+    default=next(iter(devices := get_devices()), ''),
+    type=device,
+    choices=devices,
+    help='use %(metavar)s as network device (default: %(default)s)',
+    metavar='DEVICE',
+    dest='device',
+)
+parser.add_argument(
+    '-n',
+    default=DEFAULT_OCTET,
+    type=int,
+    choices=range(2, 254),
+    help='use %(metavar)s as last ip octet for sending (default: %(default)s)',
+    metavar='NODE',
+    dest='node',
+)
+parser.add_argument(
+    '-s',
+    default=DEFAULT_SLEEP,
+    type=int,
+    help='sleep %(metavar)s ms between each request (default: %(default)s)',
+    metavar='TIME',
+    dest='sleep',
+)
+parser.add_argument(
+    '-v',
+    action='version',
+    help='show program version and exit',
+    version=__version__,
+)
+
+##################
+# Options: Modes #
+##################
+modes.add_argument(
+    '-f',
+    action='store_true',
+    help='enable fast mode, only scan specific hosts',
+    dest='f',
+)
+modes.add_argument(
+    '-F',
+    action='store_true',
+    help='enable filter mode, exclude hosts not in range',
+    dest='F',
+)
+mutual.add_argument(
+    '-p',
+    action='store_true',
+    help='enable passive mode, do not send any packets',
+    dest='p',
+)
+mutual.add_argument(
+    '-R',
+    action='store_true',
+    help='enable continuous mode, never stop sending packets',
+    dest='R',
+)
+modes.add_argument(
+    '-S',
+    action='store_true',
+    help='enable strict mode, treat inconsistent packets as new',
+    dest='S',
+)
```

### Comparing `project_harpy-0.0.10/harpy/consts.py` & `project.harpy-0.0.9/harpy/consts.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,38 +1,38 @@
-"""This file contains constants."""
-
-import re
-
-############
-# Argument #
-############
-DEFAULT_OCTET = 43
-DEFAULT_SLEEP = 1
-
-##########
-# Socket #
-##########
-GGP = 3  # https://www.iana.org/assignments/protocol-numbers
-PORT = 0  # auto
-
-##########
-# Packet #
-##########
-BUF_ETH = sum(map(int, re.findall(r'\d', (FMT_ETH := '!6s6s2s'))))
-BUF_ARP = sum(map(int, re.findall(r'\d', (FMT_ARP := '!2s2s1s1s2s6s4s6s4s'))))
-BUFSIZE = BUF_ETH + BUF_ARP
-
-##########
-# Thread #
-##########
-WAIT_PRINT = 1
-WAIT_BLOCK = .001
-
-############
-# Terminal #
-############
-CLS = '\x1b[H\x1b[2J\x1b[3J'  # https://en.wikipedia.org/wiki/ANSI_escape_code
-LOGO = (
-    r'|_  _  _ _   ',
-    r'| |(_|| |_)\/',
-    r'        |  / ',
-)
+"""This file contains constants."""
+
+import re
+
+############
+# Argument #
+############
+DEFAULT_OCTET = 43
+DEFAULT_SLEEP = 1
+
+##########
+# Socket #
+##########
+GGP = 3  # https://www.iana.org/assignments/protocol-numbers
+PORT = 0  # auto
+
+##########
+# Packet #
+##########
+BUF_ETH = sum(map(int, re.findall(r'\d', (FMT_ETH := '!6s6s2s'))))
+BUF_ARP = sum(map(int, re.findall(r'\d', (FMT_ARP := '!2s2s1s1s2s6s4s6s4s'))))
+BUFSIZE = BUF_ETH + BUF_ARP
+
+##########
+# Thread #
+##########
+WAIT_PRINT = 1
+WAIT_BLOCK = .001
+
+############
+# Terminal #
+############
+CLS = '\x1b[H\x1b[2J\x1b[3J'  # https://en.wikipedia.org/wiki/ANSI_escape_code
+LOGO = (
+    r'|_  _  _ _   ',
+    r'| |(_|| |_)\/',
+    r'        |  / ',
+)
```

### Comparing `project_harpy-0.0.10/harpy/db.json` & `project.harpy-0.0.9/harpy/db.json`

 * *Files identical despite different names*

### Comparing `project_harpy-0.0.10/harpy/handlers.py` & `project.harpy-0.0.9/harpy/handlers.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,50 +1,50 @@
-"""Various handlers."""
-
-import atexit
-import os
-import sys
-import termios
-
-
-class Echo:
-    """Terminal echo."""
-
-    @staticmethod
-    @atexit.register
-    def enable() -> None:
-        """Enable echo."""
-        try:
-            attributes = termios.tcgetattr(0)
-            attributes[3] |= termios.ECHO
-            termios.tcsetattr(0, termios.TCSANOW, attributes)
-        except termios.error:
-            pass
-
-    @staticmethod
-    def disable() -> None:
-        """Disable echo."""
-        try:
-            attributes = termios.tcgetattr(0)
-            attributes[3] &= ~termios.ECHO
-            termios.tcsetattr(0, termios.TCSANOW, attributes)
-        except termios.error:
-            pass
-
-
-class Is:
-    """Multiple unrelated "is" questions."""
-
-    @staticmethod
-    def atty() -> bool:
-        """Test if all file descriptors are connected to a terminal."""
-        return all(fd.isatty() for fd in [sys.stdin, sys.stdout, sys.stderr])
-
-    @staticmethod
-    def fore() -> bool:
-        """Test if the program is running in the foreground."""
-        return os.getpgrp() == os.tcgetpgrp(1)
-
-    @staticmethod
-    def root() -> bool:
-        """Test if user is root."""
-        return os.geteuid() == 0
+"""Various handlers."""
+
+import atexit
+import os
+import sys
+import termios
+
+
+class Echo:
+    """Terminal echo."""
+
+    @staticmethod
+    @atexit.register
+    def enable() -> None:
+        """Enable echo."""
+        try:
+            attributes = termios.tcgetattr(0)
+            attributes[3] |= termios.ECHO
+            termios.tcsetattr(0, termios.TCSANOW, attributes)
+        except termios.error:
+            pass
+
+    @staticmethod
+    def disable() -> None:
+        """Disable echo."""
+        try:
+            attributes = termios.tcgetattr(0)
+            attributes[3] &= ~termios.ECHO
+            termios.tcsetattr(0, termios.TCSANOW, attributes)
+        except termios.error:
+            pass
+
+
+class Is:
+    """Multiple unrelated "is" questions."""
+
+    @staticmethod
+    def atty() -> bool:
+        """Test if all file descriptors are connected to a terminal."""
+        return all(fd.isatty() for fd in [sys.stdin, sys.stdout, sys.stderr])
+
+    @staticmethod
+    def fore() -> bool:
+        """Test if the program is running in the foreground."""
+        return os.getpgrp() == os.tcgetpgrp(1)
+
+    @staticmethod
+    def root() -> bool:
+        """Test if user is root."""
+        return os.geteuid() == 0
```

### Comparing `project_harpy-0.0.10/harpy/net.py` & `project.harpy-0.0.9/harpy/net.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,190 +1,190 @@
-"""Custom network threads."""
-
-import binascii
-import dataclasses
-import ipaddress
-import os
-import socket
-import struct
-import textwrap
-import threading
-from itertools import cycle
-from typing import Generator
-
-from harpy.consts import (
-    BUFSIZE,
-    BUF_ETH,
-    DEFAULT_SLEEP,
-    FMT_ARP,
-    FMT_ETH,
-    WAIT_BLOCK,
-)
-from harpy.globs import controller, interrupts, sent
-from harpy.utils import get_manuf
-
-
-class Thread(threading.Thread):
-    """Base class for network threads."""
-
-    def __init__(self, so: socket.socket, nw: ipaddress.IPv4Network) -> None:
-        super().__init__()
-
-        self.sock = so
-        self.network = nw
-
-        self.src = so.getsockname()[-1].hex()
-        self.sha = self.src
-
-
-class Sender(Thread):
-    """Sender thread."""
-
-    name = 'Sender'
-
-    def __init__(self, so, nw, node: int, ms: int, f: bool, R: bool) -> None:
-        super().__init__(so, nw)
-
-        self.node = node
-        self.sleep = ms / 1000
-        self.fast = f
-        self.repeat = R
-
-        self.hosts = iter(nw.hosts()) if not R else cycle(nw.hosts())
-
-    def run(self) -> None:
-        """Method representing the thread's activity."""
-        while not controller.is_set() and (host := next(self.hosts, None)):
-            tpa = str(host)
-
-            node = int(tpa.rsplit('.', 1)[-1])
-
-            if self.fast and node not in (1, 2, 100, 127, 200, 254):
-                continue
-
-            # Fix gratuitous ARP
-            spa = str(host - node + (node != self.node) * self.node)
-
-            # https://en.wikipedia.org/wiki/Ethernet_frame
-            eth = struct.pack(
-                FMT_ETH,
-                b'\xff' * 6,  # Destination MAC Address
-                binascii.unhexlify(self.src),  # Source MAC Address
-                b'\x08\x06',  # EtherType
-            )
-
-            # https://en.wikipedia.org/wiki/Address_Resolution_Protocol
-            arp = struct.pack(
-                FMT_ARP,
-                b'\x00\x01',  # Hardware Type
-                b'\x08\x00',  # Protocol Type
-                b'\x06',  # Hardware Address Length
-                b'\x04',  # Protocol Address Length
-                b'\x00\x01',  # Operation Code
-                binascii.unhexlify(self.sha),  # Sender Hardware Address
-                socket.inet_aton(spa),  # Sender Protocol Address
-                b'\xff' * 6,  # Target Hardware Address
-                socket.inet_aton(tpa),  # Target Protocol Address
-            )
-
-            try:
-                self.sock.send(eth + arp)
-            except BlockingIOError:
-                controller.wait(WAIT_BLOCK)
-                continue
-            except OSError as err:
-                controller.set()
-                interrupts.append([self.name, err])
-                break
-            else:
-                sent.set(spa + '->' + tpa)
-                try:
-                    controller.wait(self.sleep)
-                except OverflowError:
-                    self.sleep = DEFAULT_SLEEP / 1000
-                    controller.wait(self.sleep)
-        else:
-            sent.set('')
-
-
-@dataclasses.dataclass
-class Scent:
-    """Sniff result fields."""
-
-    spa: str
-
-    who_has: int
-    is_at: int
-
-    source: dict[str, str]
-    sender: dict[str, str]
-
-
-class Sniffer(Thread):
-    """Sniffer thread."""
-
-    name = 'Sniffer'
-
-    def __init__(self, so, nw, db: dict[str, str], F: bool, S: bool) -> None:
-        super().__init__(so, nw)
-
-        self.db = db
-        self.exclude = F
-        self.strict = S
-
-        self.scents = []  # type: list[Scent]
-
-    def __iter__(self) -> Generator[str, None, None]:
-        for scent in self.scents:
-            yield textwrap.shorten(str(scent), os.get_terminal_size().columns)
-
-    def run(self) -> None:
-        """Method representing the thread's activity."""
-        while not controller.is_set():
-            try:
-                packet = self.sock.recv(BUFSIZE)
-            except BlockingIOError:
-                controller.wait(WAIT_BLOCK)  # Performance improvement!
-                continue
-            except OSError as err:
-                controller.set()
-                interrupts.append([self.name, err])
-                break
-            else:
-                if len(packet) < BUFSIZE:
-                    continue
-
-            eth = struct.unpack(FMT_ETH, packet[:BUF_ETH])
-
-            src = eth[1].hex()
-
-            if src == self.src:
-                continue
-
-            if eth[2] != b'\x08\x06':
-                continue
-
-            arp = struct.unpack(FMT_ARP, packet[BUF_ETH:BUFSIZE])
-
-            spa = socket.inet_ntoa(arp[6])
-
-            if self.exclude and ipaddress.IPv4Address(spa) not in self.network:
-                continue
-
-            who_has = int(arp[4] == b'\x00\x01')
-            is_at = 1 - who_has
-
-            sha = arp[5].hex()
-
-            source = {src: get_manuf(self.db, src)}
-            sender = {sha: get_manuf(self.db, sha)}
-
-            for scent in self.scents:
-                if (scent.spa, scent.source) == (spa, source):
-                    if self.strict:
-                        if scent.sender != sender:
-                            continue
-                    scent.who_has += who_has
-                    scent.is_at += is_at
-                    break
-            else:
-                self.scents.append(Scent(spa, who_has, is_at, source, sender))
+"""Custom network threads."""
+
+import binascii
+import dataclasses
+import ipaddress
+import os
+import socket
+import struct
+import textwrap
+import threading
+from itertools import cycle
+from typing import Generator
+
+from harpy.consts import (
+    BUFSIZE,
+    BUF_ETH,
+    DEFAULT_SLEEP,
+    FMT_ARP,
+    FMT_ETH,
+    WAIT_BLOCK,
+)
+from harpy.globs import controller, interrupts, sent
+from harpy.utils import get_manuf
+
+
+class Thread(threading.Thread):
+    """Base class for network threads."""
+
+    def __init__(self, so: socket.socket, nw: ipaddress.IPv4Network) -> None:
+        super().__init__()
+
+        self.sock = so
+        self.network = nw
+
+        self.src = so.getsockname()[-1].hex()
+        self.sha = self.src
+
+
+class Sender(Thread):
+    """Sender thread."""
+
+    name = 'Sender'
+
+    def __init__(self, so, nw, node: int, ms: int, f: bool, R: bool) -> None:
+        super().__init__(so, nw)
+
+        self.node = node
+        self.sleep = ms / 1000
+        self.fast = f
+        self.repeat = R
+
+        self.hosts = iter(nw.hosts()) if not R else cycle(nw.hosts())
+
+    def run(self) -> None:
+        """Method representing the thread's activity."""
+        while not controller.is_set() and (host := next(self.hosts, None)):
+            tpa = str(host)
+
+            node = int(tpa.rsplit('.', 1)[-1])
+
+            if self.fast and node not in (1, 2, 100, 127, 200, 254):
+                continue
+
+            # Fix gratuitous ARP
+            spa = str(host - node + (node != self.node) * self.node)
+
+            # https://en.wikipedia.org/wiki/Ethernet_frame
+            eth = struct.pack(
+                FMT_ETH,
+                b'\xff' * 6,  # Destination MAC Address
+                binascii.unhexlify(self.src),  # Source MAC Address
+                b'\x08\x06',  # EtherType
+            )
+
+            # https://en.wikipedia.org/wiki/Address_Resolution_Protocol
+            arp = struct.pack(
+                FMT_ARP,
+                b'\x00\x01',  # Hardware Type
+                b'\x08\x00',  # Protocol Type
+                b'\x06',  # Hardware Address Length
+                b'\x04',  # Protocol Address Length
+                b'\x00\x01',  # Operation Code
+                binascii.unhexlify(self.sha),  # Sender Hardware Address
+                socket.inet_aton(spa),  # Sender Protocol Address
+                b'\xff' * 6,  # Target Hardware Address
+                socket.inet_aton(tpa),  # Target Protocol Address
+            )
+
+            try:
+                self.sock.send(eth + arp)
+            except BlockingIOError:
+                controller.wait(WAIT_BLOCK)
+                continue
+            except OSError as err:
+                controller.set()
+                interrupts.append([self.name, err])
+                break
+            else:
+                sent.set(spa + '->' + tpa)
+                try:
+                    controller.wait(self.sleep)
+                except OverflowError:
+                    self.sleep = DEFAULT_SLEEP / 1000
+                    controller.wait(self.sleep)
+        else:
+            sent.set('')
+
+
+@dataclasses.dataclass
+class Scent:
+    """Sniff result fields."""
+
+    spa: str
+
+    who_has: int
+    is_at: int
+
+    source: dict[str, str]
+    sender: dict[str, str]
+
+
+class Sniffer(Thread):
+    """Sniffer thread."""
+
+    name = 'Sniffer'
+
+    def __init__(self, so, nw, db: dict[str, str], F: bool, S: bool) -> None:
+        super().__init__(so, nw)
+
+        self.db = db
+        self.exclude = F
+        self.strict = S
+
+        self.scents = []  # type: list[Scent]
+
+    def __iter__(self) -> Generator[str, None, None]:
+        for scent in self.scents:
+            yield textwrap.shorten(str(scent), os.get_terminal_size().columns)
+
+    def run(self) -> None:
+        """Method representing the thread's activity."""
+        while not controller.is_set():
+            try:
+                packet = self.sock.recv(BUFSIZE)
+            except BlockingIOError:
+                controller.wait(WAIT_BLOCK)  # Performance improvement!
+                continue
+            except OSError as err:
+                controller.set()
+                interrupts.append([self.name, err])
+                break
+            else:
+                if len(packet) < BUFSIZE:
+                    continue
+
+            eth = struct.unpack(FMT_ETH, packet[:BUF_ETH])
+
+            src = eth[1].hex()
+
+            if src == self.src:
+                continue
+
+            if eth[2] != b'\x08\x06':
+                continue
+
+            arp = struct.unpack(FMT_ARP, packet[BUF_ETH:BUFSIZE])
+
+            spa = socket.inet_ntoa(arp[6])
+
+            if self.exclude and ipaddress.IPv4Address(spa) not in self.network:
+                continue
+
+            who_has = int(arp[4] == b'\x00\x01')
+            is_at = 1 - who_has
+
+            sha = arp[5].hex()
+
+            source = {src: get_manuf(self.db, src)}
+            sender = {sha: get_manuf(self.db, sha)}
+
+            for scent in self.scents:
+                if (scent.spa, scent.source) == (spa, source):
+                    if self.strict:
+                        if scent.sender != sender:
+                            continue
+                    scent.who_has += who_has
+                    scent.is_at += is_at
+                    break
+            else:
+                self.scents.append(Scent(spa, who_has, is_at, source, sender))
```

### Comparing `project_harpy-0.0.10/harpy/utils.py` & `project.harpy-0.0.9/harpy/utils.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,58 +1,58 @@
-"""General utilities."""
-
-import json
-import os
-import signal
-import socket
-import threading
-from contextlib import contextmanager, suppress
-from typing import Generator
-
-
-def get_devices() -> list[str]:
-    """Return a list of network devices."""
-    names = []
-
-    for _, name in socket.if_nameindex():
-        if name == 'lo':
-            continue
-
-        operstate = os.path.join('/sys/class/net', name, 'operstate')
-
-        with suppress(OSError), open(operstate, 'rb') as file:
-            if file.readline().rstrip() == b'up':
-                names.append(name)
-
-    return names
-
-
-def get_manuf(manuf_db: dict[str, str], mac: str) -> str:
-    """Get a manufacturer."""
-    return manuf_db.get(mac[:6], '')
-
-
-def get_manuf_db(path: str) -> dict[str, str]:
-    """Get manufacturer database."""
-    try:
-        with open(path, encoding='utf-8') as file:
-            return json.load(file)
-    except(OSError, json.JSONDecodeError):
-        return {}
-
-
-@contextmanager
-def ignore(signum: signal.Signals) -> Generator[None, None, None]:
-    """Ignore the given signal during the execution."""
-    handler = signal.getsignal(signum)
-    safesignal(signum, signal.SIG_IGN)
-    yield
-    safesignal(signum, handler)
-
-
-def safesignal(signum: signal.Signals, handler) -> None:
-    """Thread-safe signal."""
-    if threading.current_thread() is not threading.main_thread():
-        return
-    # https://github.com/python/cpython/issues/67584
-    with suppress(TypeError):
-        signal.signal(signum, handler)
+"""General utilities."""
+
+import json
+import os
+import signal
+import socket
+import threading
+from contextlib import contextmanager, suppress
+from typing import Generator
+
+
+def get_devices() -> list[str]:
+    """Return a list of network devices."""
+    names = []
+
+    for _, name in socket.if_nameindex():
+        if name == 'lo':
+            continue
+
+        operstate = os.path.join('/sys/class/net', name, 'operstate')
+
+        with suppress(OSError), open(operstate, 'rb') as file:
+            if file.readline().rstrip() == b'up':
+                names.append(name)
+
+    return names
+
+
+def get_manuf(manuf_db: dict[str, str], mac: str) -> str:
+    """Get a manufacturer."""
+    return manuf_db.get(mac[:6], '')
+
+
+def get_manuf_db(path: str) -> dict[str, str]:
+    """Get manufacturer database."""
+    try:
+        with open(path, encoding='utf-8') as file:
+            return json.load(file)
+    except(OSError, json.JSONDecodeError):
+        return {}
+
+
+@contextmanager
+def ignore(signum: signal.Signals) -> Generator[None, None, None]:
+    """Ignore the given signal during the execution."""
+    handler = signal.getsignal(signum)
+    safesignal(signum, signal.SIG_IGN)
+    yield
+    safesignal(signum, handler)
+
+
+def safesignal(signum: signal.Signals, handler) -> None:
+    """Thread-safe signal."""
+    if threading.current_thread() is not threading.main_thread():
+        return
+    # https://github.com/python/cpython/issues/67584
+    with suppress(TypeError):
+        signal.signal(signum, handler)
```

### Comparing `project_harpy-0.0.10/project.harpy.egg-info/PKG-INFO` & `project.harpy-0.0.9/project.harpy.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-Metadata-Version: 2.1
-Name: project.harpy
-Version: 0.0.10
-Summary: Active/passive ARP discovery tool
-Author: Serhat Çelik
-License: MIT
-Keywords: harpy,arp,discovery
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Environment :: Console
-Classifier: Intended Audience :: Information Technology
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Topic :: System :: Networking
-Classifier: Topic :: System :: Networking :: Monitoring
-Requires-Python: <3.12,>=3.9
-License-File: LICENSE
+Metadata-Version: 2.1
+Name: project.harpy
+Version: 0.0.9
+Summary: Active/passive ARP discovery tool
+Author: Serhat Çelik
+License: MIT
+Keywords: harpy,arp,discovery
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Environment :: Console
+Classifier: Intended Audience :: Information Technology
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: System :: Networking
+Classifier: Topic :: System :: Networking :: Monitoring
+Requires-Python: <3.12,>=3.9
+License-File: LICENSE
```

### Comparing `project_harpy-0.0.10/pyproject.toml` & `project.harpy-0.0.9/pyproject.toml`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,37 +1,37 @@
-[build-system]
-requires = ['setuptools']
-build-backend = 'setuptools.build_meta'
-
-[project]
-name = 'project.harpy'
-authors = [{name = 'Serhat Çelik'}]
-description = 'Active/passive ARP discovery tool'
-requires-python = '>=3.9, <3.12'
-keywords = ['harpy', 'arp', 'discovery']
-license = {text = 'MIT'}
-classifiers = [
-    'Development Status :: 5 - Production/Stable',
-    'Environment :: Console',
-    'Intended Audience :: Information Technology',
-    'License :: OSI Approved :: MIT License',
-    'Programming Language :: Python :: 3',
-    'Programming Language :: Python :: 3 :: Only',
-    'Programming Language :: Python :: 3.9',
-    'Programming Language :: Python :: 3.10',
-    'Programming Language :: Python :: 3.11',
-    'Topic :: System :: Networking',
-    'Topic :: System :: Networking :: Monitoring',
-]
-dynamic = ['version']
-
-[project.scripts]
-harpy = 'harpy.__main__:main'
-
-[tool.setuptools]
-zip-safe = false
-
-[tool.setuptools.package-data]
-harpy = ['*.json']
-
-[tool.setuptools.dynamic]
-version = {attr = 'harpy.__version__.__version__'}
+[build-system]
+requires = ['setuptools']
+build-backend = 'setuptools.build_meta'
+
+[project]
+name = 'project.harpy'
+authors = [{name = 'Serhat Çelik'}]
+description = 'Active/passive ARP discovery tool'
+requires-python = '>=3.9, <3.12'
+keywords = ['harpy', 'arp', 'discovery']
+license = {text = 'MIT'}
+classifiers = [
+    'Development Status :: 5 - Production/Stable',
+    'Environment :: Console',
+    'Intended Audience :: Information Technology',
+    'License :: OSI Approved :: MIT License',
+    'Programming Language :: Python :: 3',
+    'Programming Language :: Python :: 3 :: Only',
+    'Programming Language :: Python :: 3.9',
+    'Programming Language :: Python :: 3.10',
+    'Programming Language :: Python :: 3.11',
+    'Topic :: System :: Networking',
+    'Topic :: System :: Networking :: Monitoring',
+]
+dynamic = ['version']
+
+[project.scripts]
+harpy = 'harpy.__main__:main'
+
+[tool.setuptools]
+zip-safe = false
+
+[tool.setuptools.package-data]
+harpy = ['*.json']
+
+[tool.setuptools.dynamic]
+version = {attr = 'harpy.__version__.__version__'}
```

