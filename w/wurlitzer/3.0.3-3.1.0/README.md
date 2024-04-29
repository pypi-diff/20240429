# Comparing `tmp/wurlitzer-3.0.3.tar.gz` & `tmp/wurlitzer-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wurlitzer-3.0.3.tar", last modified: Thu Dec  1 08:23:11 2022, max compression
+gzip compressed data, was "wurlitzer-3.1.0.tar", last modified: Mon Apr 29 10:39:41 2024, max compression
```

## Comparing `wurlitzer-3.0.3.tar` & `wurlitzer-3.1.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-01 08:23:11.810770 wurlitzer-3.0.3/
--rw-r--r--   0 runner    (1001) docker     (122)     5851 2022-12-01 08:22:58.000000 wurlitzer-3.0.3/Demo.ipynb
--rw-r--r--   0 runner    (1001) docker     (122)     1073 2022-12-01 08:22:58.000000 wurlitzer-3.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      125 2022-12-01 08:22:58.000000 wurlitzer-3.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     1855 2022-12-01 08:23:11.810770 wurlitzer-3.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1369 2022-12-01 08:22:58.000000 wurlitzer-3.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (122)       61 2022-12-01 08:22:58.000000 wurlitzer-3.0.3/dev-requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)      860 2022-12-01 08:22:58.000000 wurlitzer-3.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)       38 2022-12-01 08:23:11.810770 wurlitzer-3.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1449 2022-12-01 08:22:58.000000 wurlitzer-3.0.3/setup.py
--rw-r--r--   0 runner    (1001) docker     (122)     4797 2022-12-01 08:22:58.000000 wurlitzer-3.0.3/test.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-01 08:23:11.810770 wurlitzer-3.0.3/wurlitzer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     1855 2022-12-01 08:23:11.000000 wurlitzer-3.0.3/wurlitzer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      238 2022-12-01 08:23:11.000000 wurlitzer-3.0.3/wurlitzer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-12-01 08:23:11.000000 wurlitzer-3.0.3/wurlitzer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       10 2022-12-01 08:23:11.000000 wurlitzer-3.0.3/wurlitzer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)    14992 2022-12-01 08:22:58.000000 wurlitzer-3.0.3/wurlitzer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 10:39:41.315538 wurlitzer-3.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     5851 2024-04-29 10:39:34.000000 wurlitzer-3.1.0/Demo.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-29 10:39:34.000000 wurlitzer-3.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-29 10:39:34.000000 wurlitzer-3.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2476 2024-04-29 10:39:41.315538 wurlitzer-3.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1990 2024-04-29 10:39:34.000000 wurlitzer-3.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-29 10:39:34.000000 wurlitzer-3.1.0/dev-requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      860 2024-04-29 10:39:34.000000 wurlitzer-3.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 10:39:41.315538 wurlitzer-3.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1449 2024-04-29 10:39:34.000000 wurlitzer-3.1.0/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6610 2024-04-29 10:39:34.000000 wurlitzer-3.1.0/test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 10:39:41.315538 wurlitzer-3.1.0/wurlitzer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2476 2024-04-29 10:39:41.000000 wurlitzer-3.1.0/wurlitzer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-04-29 10:39:41.000000 wurlitzer-3.1.0/wurlitzer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 10:39:41.000000 wurlitzer-3.1.0/wurlitzer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-29 10:39:41.000000 wurlitzer-3.1.0/wurlitzer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    18200 2024-04-29 10:39:34.000000 wurlitzer-3.1.0/wurlitzer.py
```

### Comparing `wurlitzer-3.0.3/Demo.ipynb` & `wurlitzer-3.1.0/Demo.ipynb`

 * *Files identical despite different names*

### Comparing `wurlitzer-3.0.3/LICENSE` & `wurlitzer-3.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `wurlitzer-3.0.3/PKG-INFO` & `wurlitzer-3.1.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wurlitzer
-Version: 3.0.3
+Version: 3.1.0
 Summary: Capture C-level output in context managers
 Home-page: https://github.com/minrk/wurlitzer
 Author: Min RK
 Author-email: benjaminrk@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -56,21 +56,45 @@
 ```python
 from wurlitzer import sys_pipes
 
 with sys_pipes():
     call_some_c_function()
 ```
 
+Forward C-level output to Python Logger objects (new in 3.1).
+Each line of output will be a log message.
+
+```python
+from wurlitzer import pipes, STDOUT
+import logging
+
+logger = logging.getLogger("my.log")
+logger.setLevel(logging.INFO)
+logger.addHandler(logging.FileHandler("mycode.log"))
+
+with pipes(logger, stderr=STDOUT):
+    call_some_c_function()
+```
+
+Forward C-level output to a file (avoids GIL issues with a background thread, new in 3.1):
+
+```python
+from wurlitzer import pipes, STDOUT
+
+with open("log.txt", "ab") as f, pipes(f, stderr=STDOUT):
+    blocking_gil_holding_function()
+```
+
 Or even simpler, enable it as an IPython extension:
 
 ```
 %load_ext wurlitzer
 ```
 
-To forward all C-level output to IPython during execution.
+To forward all C-level output to IPython (e.g. Jupyter cell output) during execution.
 
 ## Acknowledgments
 
 This package is based on stuff we learned with @takluyver and @karies while working on capturing output from the [Cling Kernel](https://github.com/root-mirror/cling/tree/master/tools/Jupyter/kernel) for Jupyter.
 
 ## Wurlitzer?!
```

### Comparing `wurlitzer-3.0.3/README.md` & `wurlitzer-3.1.0/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -40,21 +40,45 @@
 ```python
 from wurlitzer import sys_pipes
 
 with sys_pipes():
     call_some_c_function()
 ```
 
+Forward C-level output to Python Logger objects (new in 3.1).
+Each line of output will be a log message.
+
+```python
+from wurlitzer import pipes, STDOUT
+import logging
+
+logger = logging.getLogger("my.log")
+logger.setLevel(logging.INFO)
+logger.addHandler(logging.FileHandler("mycode.log"))
+
+with pipes(logger, stderr=STDOUT):
+    call_some_c_function()
+```
+
+Forward C-level output to a file (avoids GIL issues with a background thread, new in 3.1):
+
+```python
+from wurlitzer import pipes, STDOUT
+
+with open("log.txt", "ab") as f, pipes(f, stderr=STDOUT):
+    blocking_gil_holding_function()
+```
+
 Or even simpler, enable it as an IPython extension:
 
 ```
 %load_ext wurlitzer
 ```
 
-To forward all C-level output to IPython during execution.
+To forward all C-level output to IPython (e.g. Jupyter cell output) during execution.
 
 ## Acknowledgments
 
 This package is based on stuff we learned with @takluyver and @karies while working on capturing output from the [Cling Kernel](https://github.com/root-mirror/cling/tree/master/tools/Jupyter/kernel) for Jupyter.
 
 ## Wurlitzer?!
```

### Comparing `wurlitzer-3.0.3/pyproject.toml` & `wurlitzer-3.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 ]
 
 [tool.tbump]
 # Uncomment this if your project is hosted on GitHub:
 github_url = "https://github.com/minrk/wurlitzer"
 
 [tool.tbump.version]
-current = "3.0.3"
+current = "3.1.0"
 
 # Example of a semver regexp.
 # Make sure this matches current_version before
 # using tbump
 regex = '''
   (?P<major>\d+)
   \.
```

### Comparing `wurlitzer-3.0.3/setup.py` & `wurlitzer-3.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `wurlitzer-3.0.3/test.py` & `wurlitzer-3.1.0/test.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding: utf-8
 from __future__ import print_function
 
 import io
+import logging
 import os
 import platform
 import sys
 import time
 from fcntl import fcntl
 from tempfile import TemporaryFile
 from unittest import mock
@@ -173,7 +174,71 @@
         assert fcntl(sys.__stdout__, wurlitzer.F_GETPIPE_SZ) == default_bufsize
         assert fcntl(sys.__stderr__, wurlitzer.F_GETPIPE_SZ) == default_bufsize
 
     bufsize = 2**18  # seems to only accept powers of two?
     with wurlitzer.pipes(bufsize=bufsize) as (stdout, stderr):
         assert fcntl(sys.__stdout__, wurlitzer.F_GETPIPE_SZ) == bufsize
         assert fcntl(sys.__stderr__, wurlitzer.F_GETPIPE_SZ) == bufsize
+
+
+def test_log_pipes(caplog):
+    with caplog.at_level(logging.INFO), wurlitzer.pipes(
+        logging.getLogger("wurlitzer.stdout"), logging.getLogger("wurlitzer.stderr")
+    ):
+        printf("some stdout")
+        printf_err("some stderr")
+
+    stdout_logs = []
+    stderr_logs = []
+    for t in caplog.record_tuples:
+        if "stdout" in t[0]:
+            stdout_logs.append(t)
+        else:
+            stderr_logs.append(t)
+
+    assert stdout_logs == [
+        ("wurlitzer.stdout", logging.INFO, "some stdout"),
+    ]
+    assert stderr_logs == [
+        ("wurlitzer.stderr", logging.ERROR, "some stderr"),
+    ]
+
+    for record in caplog.records:
+        # check 'stream' extra
+        assert record.stream
+        assert record.name == "wurlitzer." + record.stream
+
+
+def test_two_file_pipes(tmpdir):
+
+    test_stdout = tmpdir / "stdout.txt"
+    test_stderr = tmpdir / "stderr.txt"
+
+    with test_stdout.open("ab") as stdout_f, test_stderr.open("ab") as stderr_f:
+        w = Wurlitzer(stdout_f, stderr_f)
+        with w:
+            assert w.thread is None
+            printf("some stdout")
+            printf_err("some stderr")
+
+    with test_stdout.open() as f:
+        assert f.read() == "some stdout\n"
+    with test_stderr.open() as f:
+        assert f.read() == "some stderr\n"
+
+
+def test_one_file_pipe(tmpdir):
+
+    test_stdout = tmpdir / "stdout.txt"
+
+    with test_stdout.open("ab") as stdout_f:
+        stderr = io.StringIO()
+        w = Wurlitzer(stdout_f, stderr)
+        with w as (stdout, stderr):
+            assert w.thread is not None
+            printf("some stdout")
+            printf_err("some stderr")
+        assert not w.thread.is_alive()
+
+    with test_stdout.open() as f:
+        assert f.read() == "some stdout\n"
+    assert stderr.getvalue() == "some stderr\n"
```

### Comparing `wurlitzer-3.0.3/wurlitzer.egg-info/PKG-INFO` & `wurlitzer-3.1.0/wurlitzer.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wurlitzer
-Version: 3.0.3
+Version: 3.1.0
 Summary: Capture C-level output in context managers
 Home-page: https://github.com/minrk/wurlitzer
 Author: Min RK
 Author-email: benjaminrk@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -56,21 +56,45 @@
 ```python
 from wurlitzer import sys_pipes
 
 with sys_pipes():
     call_some_c_function()
 ```
 
+Forward C-level output to Python Logger objects (new in 3.1).
+Each line of output will be a log message.
+
+```python
+from wurlitzer import pipes, STDOUT
+import logging
+
+logger = logging.getLogger("my.log")
+logger.setLevel(logging.INFO)
+logger.addHandler(logging.FileHandler("mycode.log"))
+
+with pipes(logger, stderr=STDOUT):
+    call_some_c_function()
+```
+
+Forward C-level output to a file (avoids GIL issues with a background thread, new in 3.1):
+
+```python
+from wurlitzer import pipes, STDOUT
+
+with open("log.txt", "ab") as f, pipes(f, stderr=STDOUT):
+    blocking_gil_holding_function()
+```
+
 Or even simpler, enable it as an IPython extension:
 
 ```
 %load_ext wurlitzer
 ```
 
-To forward all C-level output to IPython during execution.
+To forward all C-level output to IPython (e.g. Jupyter cell output) during execution.
 
 ## Acknowledgments
 
 This package is based on stuff we learned with @takluyver and @karies while working on capturing output from the [Cling Kernel](https://github.com/root-mirror/cling/tree/master/tools/Jupyter/kernel) for Jupyter.
 
 ## Wurlitzer?!
```

### Comparing `wurlitzer-3.0.3/wurlitzer.py` & `wurlitzer-3.1.0/wurlitzer.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 """Capture C-level FD output on pipes
 
 Use `wurlitzer.pipes` or `wurlitzer.sys_pipes` as context managers.
 """
+
 from __future__ import print_function
 
-__version__ = '3.0.3'
+__version__ = '3.1.0'
 
 __all__ = [
     'pipes',
     'sys_pipes',
     'sys_pipes_forever',
     'stop_sys_pipes',
     'PIPE',
     'STDOUT',
     'Wurlitzer',
 ]
 
 import ctypes
 import errno
 import io
+import logging
 import os
 import platform
 import selectors
 import sys
 import threading
 import time
 import warnings
@@ -178,14 +180,20 @@
         encoding: str or None
             The encoding to use, if streams should be interpreted as text.
         bufsize: int or None
             Set pipe buffer size using fcntl F_SETPIPE_SZ (linux only)
             default: use /proc/sys/fs/pipe-max-size up to a max of 1MB
             if 0, will do nothing.
         """
+        # accept logger objects
+        if stdout and isinstance(stdout, logging.Logger):
+            stdout = _LogPipe(stdout, stream_name="stdout", level=logging.INFO)
+        if stderr and isinstance(stderr, logging.Logger):
+            stderr = _LogPipe(stderr, stream_name="stderr", level=logging.ERROR)
+
         self._stdout = stdout
         if stderr == STDOUT:
             self._stderr = self._stdout
         else:
             self._stderr = stderr
         self.encoding = encoding
         if bufsize is None:
@@ -198,14 +206,25 @@
         self._handlers['stdout'] = self._handle_stdout
 
     def _setup_pipe(self, name):
         real_fd = getattr(sys, '__%s__' % name).fileno()
         save_fd = os.dup(real_fd)
         self._save_fds[name] = save_fd
 
+        try:
+            capture_fd = getattr(self, "_" + name).fileno()
+        except Exception:
+            pass
+        else:
+            # if it has a fileno(),
+            # dup directly to capture file,
+            # no pipes needed
+            dup2(capture_fd, real_fd)
+            return None
+
         pipe_out, pipe_in = os.pipe()
         # set max pipe buffer size (linux only)
         if self._bufsize:
             try:
                 fcntl(pipe_in, F_SETPIPE_SZ, self._bufsize)
             except OSError as error:
                 warnings.warn(
@@ -260,27 +279,40 @@
             libc.fflush(c_stderr_p)
 
     def __enter__(self):
         # flush anything out before starting
         self._flush()
         # setup handle
         self._setup_handle()
-        self._control_r, self._control_w = os.pipe()
 
         # create pipe for stdout
-        pipes = [self._control_r]
-        names = {self._control_r: 'control'}
+        pipes = []
+        names = {}
         if self._stdout:
             pipe = self._setup_pipe('stdout')
-            pipes.append(pipe)
-            names[pipe] = 'stdout'
+            if pipe:
+                pipes.append(pipe)
+                names[pipe] = 'stdout'
         if self._stderr:
             pipe = self._setup_pipe('stderr')
-            pipes.append(pipe)
-            names[pipe] = 'stderr'
+            if pipe:
+                pipes.append(pipe)
+                names[pipe] = 'stderr'
+
+        if not pipes:
+            # no pipes to handle (e.g. direct FD capture)
+            # so no forwarder thread needed
+            self.thread = None
+            return self.handle
+
+        # setup forwarder thread
+
+        self._control_r, self._control_w = os.pipe()
+        pipes.append(self._control_r)
+        names[self._control_r] = "control"
 
         # flush pipes in a background thread to avoid blocking
         # the reader thread when the buffer is full
         flush_queue = Queue()
 
         def flush_main():
             while True:
@@ -354,19 +386,19 @@
         self.thread.start()
 
         return self.handle
 
     def __exit__(self, exc_type, exc_value, traceback):
         # flush before exiting
         self._flush()
-
-        # signal output is complete on control pipe
-        os.write(self._control_w, b'\1')
-        self.thread.join()
-        os.close(self._control_w)
+        if self.thread:
+            # signal output is complete on control pipe
+            os.write(self._control_w, b'\1')
+            self.thread.join()
+            os.close(self._control_w)
 
         # restore original state
         for name, real_fd in self._real_fds.items():
             save_fd = self._save_fds[name]
             dup2(save_fd, real_fd)
             os.close(save_fd)
         # finalize handle
@@ -375,34 +407,53 @@
 
 @contextmanager
 def pipes(stdout=PIPE, stderr=PIPE, encoding=_default_encoding, bufsize=None):
     """Capture C-level stdout/stderr in a context manager.
 
     The return value for the context manager is (stdout, stderr).
 
+    Args:
+
+    stdout (optional, default: PIPE): None or PIPE or Writable or Logger
+    stderr (optional, default: PIPE): None or PIPE or STDOUT or Writable or Logger
+    encoding (optional): probably 'utf-8'
+    bufsize (optional): set explicit buffer size if the default doesn't work
+
+    .. versionadded:: 3.1
+        Accept Logger objects for stdout/stderr.
+        If a Logger is specified, each line will produce a log message.
+        stdout messages will be at INFO level, stderr messages at ERROR level.
+
     .. versionchanged:: 3.0
 
         when using `PIPE` (default), the type of captured output
         is `io.StringIO/BytesIO` instead of an OS pipe.
         This eliminates max buffer size issues (and hang when output exceeds 65536 bytes),
         but also means the buffer cannot be read with `.read()` methods
         until after the context exits.
 
     Examples
     --------
 
-    >>> with capture() as (stdout, stderr):
+    >>> with pipes() as (stdout, stderr):
     ...     printf("C-level stdout")
     ... output = stdout.read()
     """
     stdout_pipe = stderr_pipe = False
     if encoding:
         PipeIO = io.StringIO
     else:
         PipeIO = io.BytesIO
+
+    # accept logger objects
+    if stdout and isinstance(stdout, logging.Logger):
+        stdout = _LogPipe(stdout, stream_name="stdout", level=logging.INFO)
+    if stderr and isinstance(stderr, logging.Logger):
+        stderr = _LogPipe(stderr, stream_name="stderr", level=logging.ERROR)
+
     # setup stdout
     if stdout == PIPE:
         stdout_r = stdout_w = PipeIO()
         stdout_pipe = True
     else:
         stdout_r = stdout_w = stdout
     # setup stderr
@@ -415,23 +466,73 @@
     else:
         stderr_r = stderr_w = stderr
     w = Wurlitzer(stdout=stdout_w, stderr=stderr_w, encoding=encoding, bufsize=bufsize)
     try:
         with w:
             yield stdout_r, stderr_r
     finally:
+        if stdout and isinstance(stdout, _LogPipe):
+            stdout.flush()
+        if stderr and isinstance(stderr, _LogPipe):
+            stderr.flush()
         # close pipes
         if stdout_pipe:
             # seek to 0 so that it can be read after exit
             stdout_r.seek(0)
         if stderr_pipe:
             # seek to 0 so that it can be read after exit
             stderr_r.seek(0)
 
 
+class _LogPipe(io.BufferedWriter):
+    """Writeable that writes lines to a Logger object as they arrive from captured pipes"""
+
+    def __init__(self, logger, stream_name, level=logging.INFO):
+        self.logger = logger
+        self.stream_name = stream_name
+        self._buf = ""
+        self.level = level
+
+    def _log(self, line):
+        """Log one line"""
+        self.logger.log(self.level, line.rstrip(), extra={"stream": self.stream_name})
+
+    def write(self, chunk):
+        """Given chunk, split into lines
+
+        Log each line as a discrete message
+
+        If it ends with a partial line, save it until the next one
+        """
+        lines = chunk.splitlines(True)
+        if self._buf:
+            lines[0] = self._buf + lines[0]
+        if lines[-1].endswith("\n"):
+            self._buf = ""
+        else:
+            # last line is incomplete
+            self._buf = lines[-1]
+            lines = lines[:-1]
+
+        for line in lines:
+            self._log(line)
+
+    def flush(self):
+        """Write buffer as a last message if there is one"""
+        if self._buf:
+            self._log(self._buf)
+            self._buf = ""
+
+    def __enter__(self):
+        return self
+
+    def __exit__(self, *exc_info):
+        self.flush()
+
+
 def sys_pipes(encoding=_default_encoding, bufsize=None):
     """Redirect C-level stdout/stderr to sys.stdout/stderr
 
     This is useful of sys.sdout/stderr are already being forwarded somewhere.
 
     DO NOT USE THIS if sys.stdout and sys.stderr are not already being forwarded.
     """
```

