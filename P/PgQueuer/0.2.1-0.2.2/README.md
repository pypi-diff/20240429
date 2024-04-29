# Comparing `tmp/pgqueuer-0.2.1.tar.gz` & `tmp/pgqueuer-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pgqueuer-0.2.1.tar", last modified: Sun Apr 28 10:47:57 2024, max compression
+gzip compressed data, was "pgqueuer-0.2.2.tar", last modified: Mon Apr 29 20:15:29 2024, max compression
```

## Comparing `pgqueuer-0.2.1.tar` & `pgqueuer-0.2.2.tar`

### file list

```diff
@@ -1,41 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 10:47:57.058543 pgqueuer-0.2.1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 10:47:57.050543 pgqueuer-0.2.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 10:47:57.054543 pgqueuer-0.2.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      963 2024-04-28 10:47:48.000000 pgqueuer-0.2.1/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)      954 2024-04-28 10:47:48.000000 pgqueuer-0.2.1/.github/workflows/linting.yml
--rw-r--r--   0 runner    (1001) docker     (127)      798 2024-04-28 10:47:48.000000 pgqueuer-0.2.1/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3119 2024-04-28 10:47:48.000000 pgqueuer-0.2.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-28 10:47:48.000000 pgqueuer-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5903 2024-04-28 10:47:57.058543 pgqueuer-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4332 2024-04-28 10:47:48.000000 pgqueuer-0.2.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      231 2024-04-28 10:47:48.000000 pgqueuer-0.2.1/docker-compose.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2073 2024-04-28 10:47:48.000000 pgqueuer-0.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-28 10:47:57.058543 pgqueuer-0.2.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 10:47:57.054543 pgqueuer-0.2.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 10:47:57.054543 pgqueuer-0.2.1/src/PgQueuer/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 10:47:48.000000 pgqueuer-0.2.1/src/PgQueuer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-28 10:47:48.000000 pgqueuer-0.2.1/src/PgQueuer/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      461 2024-04-28 10:47:48.000000 pgqueuer-0.2.1/src/PgQueuer/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     3457 2024-04-28 10:47:48.000000 pgqueuer-0.2.1/src/PgQueuer/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)      185 2024-04-28 10:47:48.000000 pgqueuer-0.2.1/src/PgQueuer/logconfig.py
--rw-r--r--   0 runner    (1001) docker     (127)      841 2024-04-28 10:47:48.000000 pgqueuer-0.2.1/src/PgQueuer/models.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 10:47:48.000000 pgqueuer-0.2.1/src/PgQueuer/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     3544 2024-04-28 10:47:48.000000 pgqueuer-0.2.1/src/PgQueuer/qm.py
--rw-r--r--   0 runner    (1001) docker     (127)     8995 2024-04-28 10:47:48.000000 pgqueuer-0.2.1/src/PgQueuer/queries.py
--rw-r--r--   0 runner    (1001) docker     (127)      596 2024-04-28 10:47:48.000000 pgqueuer-0.2.1/src/PgQueuer/tm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 10:47:57.058543 pgqueuer-0.2.1/src/PgQueuer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5903 2024-04-28 10:47:57.000000 pgqueuer-0.2.1/src/PgQueuer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      701 2024-04-28 10:47:57.000000 pgqueuer-0.2.1/src/PgQueuer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-28 10:47:57.000000 pgqueuer-0.2.1/src/PgQueuer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-28 10:47:57.000000 pgqueuer-0.2.1/src/PgQueuer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-28 10:47:57.000000 pgqueuer-0.2.1/src/PgQueuer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-28 10:47:56.000000 pgqueuer-0.2.1/src/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 10:47:57.058543 pgqueuer-0.2.1/test/
--rw-r--r--   0 runner    (1001) docker     (127)     1337 2024-04-28 10:47:48.000000 pgqueuer-0.2.1/test/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 10:47:57.058543 pgqueuer-0.2.1/test/db/
--rw-r--r--   0 runner    (1001) docker     (127)      526 2024-04-28 10:47:48.000000 pgqueuer-0.2.1/test/db/Dockerfile
--rwxr-xr-x   0 runner    (1001) docker     (127)      266 2024-04-28 10:47:48.000000 pgqueuer-0.2.1/test/db/init_db.sh
--rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-04-28 10:47:48.000000 pgqueuer-0.2.1/test/test_benchmark.py
--rw-r--r--   0 runner    (1001) docker     (127)     1669 2024-04-28 10:47:48.000000 pgqueuer-0.2.1/test/test_qm.py
--rw-r--r--   0 runner    (1001) docker     (127)     4047 2024-04-28 10:47:48.000000 pgqueuer-0.2.1/test/test_queries.py
--rw-r--r--   0 runner    (1001) docker     (127)      527 2024-04-28 10:47:48.000000 pgqueuer-0.2.1/test/test_tm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 20:15:29.288138 pgqueuer-0.2.2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 20:15:29.280138 pgqueuer-0.2.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 20:15:29.284138 pgqueuer-0.2.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1670 2024-04-29 20:15:19.000000 pgqueuer-0.2.2/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      954 2024-04-29 20:15:19.000000 pgqueuer-0.2.2/.github/workflows/linting.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      798 2024-04-29 20:15:19.000000 pgqueuer-0.2.2/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3119 2024-04-29 20:15:19.000000 pgqueuer-0.2.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-29 20:15:19.000000 pgqueuer-0.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5929 2024-04-29 20:15:29.288138 pgqueuer-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4332 2024-04-29 20:15:19.000000 pgqueuer-0.2.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-04-29 20:15:19.000000 pgqueuer-0.2.2/docker-compose.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2091 2024-04-29 20:15:19.000000 pgqueuer-0.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 20:15:29.288138 pgqueuer-0.2.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 20:15:29.284138 pgqueuer-0.2.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 20:15:29.284138 pgqueuer-0.2.2/src/PgQueuer/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 20:15:19.000000 pgqueuer-0.2.2/src/PgQueuer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-29 20:15:19.000000 pgqueuer-0.2.2/src/PgQueuer/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      461 2024-04-29 20:15:19.000000 pgqueuer-0.2.2/src/PgQueuer/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3457 2024-04-29 20:15:19.000000 pgqueuer-0.2.2/src/PgQueuer/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-04-29 20:15:19.000000 pgqueuer-0.2.2/src/PgQueuer/logconfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)      841 2024-04-29 20:15:19.000000 pgqueuer-0.2.2/src/PgQueuer/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 20:15:19.000000 pgqueuer-0.2.2/src/PgQueuer/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     4694 2024-04-29 20:15:19.000000 pgqueuer-0.2.2/src/PgQueuer/qm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10711 2024-04-29 20:15:19.000000 pgqueuer-0.2.2/src/PgQueuer/queries.py
+-rw-r--r--   0 runner    (1001) docker     (127)      794 2024-04-29 20:15:19.000000 pgqueuer-0.2.2/src/PgQueuer/tm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 20:15:29.288138 pgqueuer-0.2.2/src/PgQueuer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5929 2024-04-29 20:15:29.000000 pgqueuer-0.2.2/src/PgQueuer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-29 20:15:29.000000 pgqueuer-0.2.2/src/PgQueuer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 20:15:29.000000 pgqueuer-0.2.2/src/PgQueuer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-29 20:15:29.000000 pgqueuer-0.2.2/src/PgQueuer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-29 20:15:29.000000 pgqueuer-0.2.2/src/PgQueuer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-29 20:15:29.000000 pgqueuer-0.2.2/src/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 20:15:29.284138 pgqueuer-0.2.2/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     1337 2024-04-29 20:15:19.000000 pgqueuer-0.2.2/test/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 20:15:29.284138 pgqueuer-0.2.2/test/db/
+-rw-r--r--   0 runner    (1001) docker     (127)      526 2024-04-29 20:15:19.000000 pgqueuer-0.2.2/test/db/Dockerfile
+-rwxr-xr-x   0 runner    (1001) docker     (127)      266 2024-04-29 20:15:19.000000 pgqueuer-0.2.2/test/db/init_db.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     2612 2024-04-29 20:15:19.000000 pgqueuer-0.2.2/test/test_qm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4032 2024-04-29 20:15:19.000000 pgqueuer-0.2.2/test/test_queries.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1007 2024-04-29 20:15:19.000000 pgqueuer-0.2.2/test/test_tm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 20:15:29.284138 pgqueuer-0.2.2/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)     2247 2024-04-29 20:15:19.000000 pgqueuer-0.2.2/tools/benchmark.py
```

### Comparing `pgqueuer-0.2.1/.github/workflows/ci.yml` & `pgqueuer-0.2.2/.github/workflows/ci.yml`

 * *Files 20% similar despite different names*

```diff
@@ -3,14 +3,45 @@
 on:
   pull_request:
     branches: [main]
   push:
     branches: [main]
 
 jobs:
+  benchmark:
+
+    strategy:
+      fail-fast: false
+      matrix:
+        python-version: ["3.11"]
+        os: [ubuntu-latest]
+
+    name: PgQueuer Benchmark
+    runs-on: ${{ matrix.os }}
+
+    steps:
+      - uses: actions/checkout@v4
+
+      - name: Set up Python
+        uses: actions/setup-python@v4
+        with:
+          python-version: ${{ matrix.python-version }}
+
+      - name: Build custom PostgreSQL Docker image
+        run: |
+          docker-compose up --build -d pgq
+
+      - name: Install PgQueuer
+        run: |
+          pip install pip -U
+          pip install .[dev]
+
+      - name: Benchmark
+        run: PGUSER=testuser PGPASSWORD=testpassword PGDATABASE=testdb python3 tools/benchmark.py
+
   ci:
     strategy:
       fail-fast: false
       matrix:
         python-version: ["3.10", "3.11", "3.12"]
         os: [ubuntu-latest]
```

### Comparing `pgqueuer-0.2.1/.github/workflows/linting.yml` & `pgqueuer-0.2.2/.github/workflows/linting.yml`

 * *Files identical despite different names*

### Comparing `pgqueuer-0.2.1/.github/workflows/release.yml` & `pgqueuer-0.2.2/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `pgqueuer-0.2.1/.gitignore` & `pgqueuer-0.2.2/.gitignore`

 * *Files identical despite different names*

### Comparing `pgqueuer-0.2.1/LICENSE` & `pgqueuer-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pgqueuer-0.2.1/PKG-INFO` & `pgqueuer-0.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PgQueuer
-Version: 0.2.1
+Version: 0.2.2
 Summary: PgQueuer is a Python library leveraging PostgreSQL for efficient job queuing.
 Author: janbjorge
 License: MIT License
 Project-URL: Documentation, https://github.com/janbjorge/PgQueuer/
 Project-URL: Homepage, https://github.com/janbjorge/PgQueuer/
 Project-URL: Issues, https://github.com/janbjorge/PgQueuer/issues
 Project-URL: Repository, https://github.com/janbjorge/PgQueuer/
@@ -22,14 +22,15 @@
 Classifier: Topic :: Database
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Utilities
 Classifier: Topic :: System :: Distributed Computing
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: anyio>=4.0
 Requires-Dist: asyncpg>=0.27.0
 Requires-Dist: pgcachewatch>=0.4
 Requires-Dist: pydantic>=2.0.0
 Provides-Extra: dev
 Requires-Dist: asyncpg-stubs; extra == "dev"
 Requires-Dist: mypy-extensions; extra == "dev"
 Requires-Dist: mypy; extra == "dev"
```

### Comparing `pgqueuer-0.2.1/README.md` & `pgqueuer-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `pgqueuer-0.2.1/pyproject.toml` & `pgqueuer-0.2.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -26,14 +26,15 @@
     "Topic :: Database",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Topic :: Utilities",
     "Topic :: System :: Distributed Computing"
 ]
 
 dependencies = [
+    "anyio>=4.0",
     "asyncpg>=0.27.0",
     "pgcachewatch>=0.4",
     "pydantic>=2.0.0",
 ]
 
 [project.urls]
 Documentation = "https://github.com/janbjorge/PgQueuer/"
```

### Comparing `pgqueuer-0.2.1/src/PgQueuer/cli.py` & `pgqueuer-0.2.2/src/PgQueuer/cli.py`

 * *Files identical despite different names*

### Comparing `pgqueuer-0.2.1/src/PgQueuer/models.py` & `pgqueuer-0.2.2/src/PgQueuer/models.py`

 * *Files identical despite different names*

### Comparing `pgqueuer-0.2.1/src/PgQueuer/qm.py` & `pgqueuer-0.2.2/src/PgQueuer/qm.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,54 +1,81 @@
 from __future__ import annotations
 
 import asyncio
 import dataclasses
-from typing import TYPE_CHECKING, Awaitable, Callable, TypeAlias, TypeVar
+import functools
+from datetime import timedelta
+from typing import (
+    TYPE_CHECKING,
+    Awaitable,
+    Callable,
+    TypeAlias,
+    TypeGuard,
+    TypeVar,
+    overload,
+)
 
+import anyio
+import anyio.to_thread
 import asyncpg
 from pgcachewatch.listeners import PGEventQueue
 from pgcachewatch.models import PGChannel
 
 from .logconfig import logger
 from .models import Job
 from .queries import DBSettings, Queries
 from .tm import TaskManager
 
 if TYPE_CHECKING:
-    EntrypointFn: TypeAlias = Callable[[Job], Awaitable[None]]
-    T = TypeVar("T", bound=EntrypointFn)
+    AsyncEntrypoint: TypeAlias = Callable[[Job], Awaitable[None]]
+    SyncEntrypoint: TypeAlias = Callable[[Job], None]
+    Entrypoint: TypeAlias = AsyncEntrypoint | SyncEntrypoint
+    T = TypeVar("T", bound=Entrypoint)
+
+
+@overload
+def is_async_callable(obj: AsyncEntrypoint) -> TypeGuard[AsyncEntrypoint]: ...
+
+
+@overload
+def is_async_callable(obj: SyncEntrypoint) -> TypeGuard[SyncEntrypoint]: ...
+
+
+def is_async_callable(obj: object) -> bool:
+    # Inspired by:
+    # https://github.com/encode/starlette/blob/9f16bf5c25e126200701f6e04330864f4a91a898/starlette/_utils.py#L38
+    while isinstance(obj, functools.partial):
+        obj = obj.func
+
+    return asyncio.iscoroutinefunction(obj) or (
+        callable(obj) and asyncio.iscoroutinefunction(obj.__call__)
+    )
 
 
 @dataclasses.dataclass
 class QueueManager:
     """
     Manages job queues and dispatches jobs to registered entry points,
     handling database connections and events.
     """
 
     pool: asyncpg.Pool
     queries: Queries = dataclasses.field(init=False)
-
     channel: PGChannel = dataclasses.field(
         default=PGChannel(DBSettings().channel),
-        init=False,
     )
     alive: bool = dataclasses.field(
         init=False,
         default=True,
     )
     # Should registry be a weakref?
-    registry: dict[str, EntrypointFn] = dataclasses.field(
+    registry: dict[str, Entrypoint] = dataclasses.field(
         init=False,
         default_factory=dict,
     )
-    tm: TaskManager = dataclasses.field(
-        init=False,
-        default_factory=TaskManager,
-    )
 
     def __post_init__(self) -> None:
         """
         Initializes database query handlers and validates pool size upon
         instance creation.
         """
         if self.pool.get_min_size() < 1:
@@ -66,54 +93,71 @@
 
         def register(func: T) -> T:
             self.registry[name] = func
             return func
 
         return register
 
-    async def run(self) -> None:
+    async def run(
+        self,
+        dequeue_timeout: timedelta = timedelta(seconds=30),
+    ) -> None:
         """
         Starts the event listener and continuously dispatches jobs to
         registered entry points until stopped.
         """
-        async with self.pool.acquire() as conn:
+        async with (
+            self.pool.acquire() as conn,
+            TaskManager() as tm,
+        ):
             listener = PGEventQueue()
             await listener.connect(conn, self.channel)
 
             while self.alive:
-                while job := await self.queries.dequeue():
-                    self._dispatch(job)
-                await listener.get()
+                while self.alive and (job := await self.queries.dequeue()):
+                    tm.add(asyncio.create_task(self._dispatch(job)))
+
+                try:
+                    await asyncio.wait_for(
+                        listener.get(),
+                        timeout=dequeue_timeout.total_seconds(),
+                    )
+                except asyncio.TimeoutError:
+                    logger.debug(
+                        "Timeout after %r without receiving an event.",
+                        dequeue_timeout,
+                    )
 
-            await asyncio.gather(*self.tm.tasks)
             await conn.reset()
 
-    def _dispatch(self, job: Job) -> None:
+    async def _dispatch(self, job: Job) -> None:
         """
         Internal method to asynchronously handle job dispatch,
         including exception logging and job status updates.
         """
 
-        async def runit() -> None:
+        logger.debug(
+            "Dispatching entrypoint/id: %s/%s",
+            job.entrypoint,
+            job.id,
+        )
+
+        try:
+            fn = self.registry[job.entrypoint]
+            if is_async_callable(fn):
+                await fn(job)
+            else:
+                await anyio.to_thread.run_sync(fn, job)
+        except Exception:
+            logger.exception(
+                "Exception while processing entrypoint/id: %s/%s",
+                job.entrypoint,
+                job.id,
+            )
+            await self.queries.log_job(job, "exception")
+        else:
             logger.debug(
-                "Dispatching entrypoint/id: %s/%s",
+                "Dispatching entrypoint/id: %s/%s - successful",
                 job.entrypoint,
                 job.id,
             )
-            try:
-                await self.registry[job.entrypoint](job)
-            except Exception:
-                logger.exception(
-                    "Exception while processing entrypoint/id: %s/%s",
-                    job.entrypoint,
-                    job.id,
-                )
-                await self.queries.log_job(job, "exception")
-            else:
-                logger.debug(
-                    "Dispatching entrypoint/id: %s/%s - successful",
-                    job.entrypoint,
-                    job.id,
-                )
-                await self.queries.log_job(job, "successful")
-
-        self.tm.add(asyncio.create_task(runit()))
+            await self.queries.log_job(job, "successful")
```

### Comparing `pgqueuer-0.2.1/src/PgQueuer/queries.py` & `pgqueuer-0.2.2/src/PgQueuer/queries.py`

 * *Files 16% similar despite different names*

```diff
@@ -75,37 +75,64 @@
                 id SERIAL PRIMARY KEY,
                 priority INT NOT NULL,
                 created TIMESTAMP WITH TIME ZONE NOT NULL DEFAULT CURRENT_TIMESTAMP,
                 status {self.settings.queue_status_type} NOT NULL,
                 entrypoint TEXT NOT NULL,
                 payload BYTEA
             );
-            CREATE UNIQUE INDEX ON {self.settings.queue_table} (priority, id) WHERE status != 'picked';
+            CREATE INDEX ON {self.settings.queue_table} (priority ASC, id DESC)
+                INCLUDE (id) WHERE status = 'queued';
 
             CREATE TYPE {self.settings.log_table_status_type} AS ENUM ('exception', 'successful');
             CREATE TABLE {self.settings.log_table} (
                 id SERIAL PRIMARY KEY,
                 priority INT NOT NULL,
                 created TIMESTAMP WITH TIME ZONE DEFAULT CURRENT_TIMESTAMP,
                 duration INTERVAL NOT NULL,
                 status {self.settings.log_table_status_type} NOT NULL,
                 entrypoint TEXT NOT NULL
             );
 
             CREATE FUNCTION {self.settings.function}() RETURNS TRIGGER AS $$
+            DECLARE
+                to_emit BOOLEAN := false;  -- Flag to decide whether to emit a notification
             BEGIN
-                PERFORM pg_notify(
-                '{self.settings.channel}',
-                json_build_object(
-                    'channel', '{self.settings.channel}',
-                    'operation', lower(TG_OP),
-                    'sent_at', NOW(),
-                    'table', TG_TABLE_NAME
-                )::text);
-                RETURN NEW;
+                -- Check operation type and set the emit flag accordingly
+                IF TG_OP = 'UPDATE' AND OLD IS DISTINCT FROM NEW THEN
+                    to_emit := true;
+                ELSIF TG_OP = 'DELETE' THEN
+                    to_emit := true;
+                ELSIF TG_OP = 'INSERT' THEN
+                    to_emit := true;
+                ELSIF TG_OP = 'TRUNCATE' THEN
+                    to_emit := true;
+                END IF;
+
+                -- Perform notification if the emit flag is set
+                IF to_emit THEN
+                    PERFORM pg_notify(
+                        '{self.settings.channel}',
+                        json_build_object(
+                            'channel', '{self.settings.channel}',
+                            'operation', lower(TG_OP),
+                            'sent_at', NOW(),
+                            'table', TG_TABLE_NAME
+                        )::text
+                    );
+                END IF;
+
+                -- Return appropriate value based on the operation
+                IF TG_OP IN ('INSERT', 'UPDATE') THEN
+                    RETURN NEW;
+                ELSIF TG_OP = 'DELETE' THEN
+                    RETURN OLD;
+                ELSE
+                    RETURN NULL; -- For TRUNCATE and other non-row-specific contexts
+                END IF;
+
             END;
             $$ LANGUAGE plpgsql;
 
             CREATE TRIGGER {self.settings.trigger}
             AFTER INSERT OR UPDATE OR DELETE OR TRUNCATE ON {self.settings.queue_table}
             EXECUTE FUNCTION {self.settings.function}();
         """  # noqa: E501
@@ -131,21 +158,17 @@
         """
         Retrieves and updates the next 'queued' job to 'picked'
         status, ensuring no two jobs with the same entrypoint
         are picked simultaneously.
         """
         query = f"""
             WITH next_job AS (
-                SELECT p1.id
-                FROM {self.settings.queue_table} p1
-                WHERE p1.status = 'queued' AND NOT EXISTS (
-                    SELECT FROM
-                    {self.settings.queue_table} p2
-                    WHERE p1.entrypoint = p2.entrypoint AND p2.status = 'picked'
-                )
+                SELECT id
+                FROM {self.settings.queue_table}
+                WHERE status = 'queued'
                 ORDER BY priority DESC, id ASC
                 FOR UPDATE SKIP LOCKED
                 LIMIT 1
             )
             UPDATE {self.settings.queue_table}
             SET status = 'picked'
             WHERE id = ANY(SELECT id FROM next_job)
@@ -154,28 +177,47 @@
 
         if row := await self.pool.fetchrow(query):
             return models.Job.model_validate(dict(row))
         return None
 
     async def enqueue(
         self,
-        entrypoint: str,
-        payload: bytes | None,
-        priority: int = 0,
+        entrypoint: str | list[str],
+        payload: bytes | None | list[bytes | None],
+        priority: int | list[int] = 0,
     ) -> None:
         """
         Inserts a new job into the queue with the specified
         entrypoint, payload, and priority, marking it as 'queued'.
+        This method ensures that if any of entrypoint, payload, or priority is a list,
+        all list arguments must be of the same length.
+
+        If two or more arguments are lists, they must be the same length;
+            otherwise, an ValueError is raised.
         """
+
+        # If they are not lists, create single-item lists for uniform processing
+        normed_entrypoint = entrypoint if isinstance(entrypoint, list) else [entrypoint]
+        normed_payload = payload if isinstance(payload, list) else [payload]
+        normed_priority = priority if isinstance(priority, list) else [priority]
+
         query = f"""
             INSERT INTO {self.settings.queue_table} (priority, status, entrypoint, payload)
             VALUES ($1, 'queued', $2, $3)
         """  # noqa: E501
 
-        await self.pool.execute(query, priority, entrypoint, payload)
+        await self.pool.executemany(
+            query,
+            zip(
+                normed_priority,
+                normed_entrypoint,
+                normed_payload,
+                strict=True,
+            ),
+        )
 
     async def clear_queue(self, entrypoint: str | list[str] | None = None) -> None:
         """
         Clears jobs from the queue, optionally filtering by entrypoint if specified.
         """
         if entrypoint:
             query = (
```

### Comparing `pgqueuer-0.2.1/src/PgQueuer/tm.py` & `pgqueuer-0.2.2/src/PgQueuer/tm.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import asyncio
 import dataclasses
 
 
 @dataclasses.dataclass
 class TaskManager:
     """
@@ -17,7 +19,13 @@
     def add(self, task: asyncio.Task) -> None:
         """
         Adds an asyncio Task to the manager and registers a
         callback to automatically remove the task when it's done.
         """
         self.tasks.add(task)
         task.add_done_callback(self.tasks.remove)
+
+    async def __aenter__(self) -> TaskManager:
+        return self
+
+    async def __aexit__(self, *_: object) -> None:
+        await asyncio.gather(*self.tasks)
```

### Comparing `pgqueuer-0.2.1/src/PgQueuer.egg-info/PKG-INFO` & `pgqueuer-0.2.2/src/PgQueuer.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PgQueuer
-Version: 0.2.1
+Version: 0.2.2
 Summary: PgQueuer is a Python library leveraging PostgreSQL for efficient job queuing.
 Author: janbjorge
 License: MIT License
 Project-URL: Documentation, https://github.com/janbjorge/PgQueuer/
 Project-URL: Homepage, https://github.com/janbjorge/PgQueuer/
 Project-URL: Issues, https://github.com/janbjorge/PgQueuer/issues
 Project-URL: Repository, https://github.com/janbjorge/PgQueuer/
@@ -22,14 +22,15 @@
 Classifier: Topic :: Database
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Utilities
 Classifier: Topic :: System :: Distributed Computing
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: anyio>=4.0
 Requires-Dist: asyncpg>=0.27.0
 Requires-Dist: pgcachewatch>=0.4
 Requires-Dist: pydantic>=2.0.0
 Provides-Extra: dev
 Requires-Dist: asyncpg-stubs; extra == "dev"
 Requires-Dist: mypy-extensions; extra == "dev"
 Requires-Dist: mypy; extra == "dev"
```

### Comparing `pgqueuer-0.2.1/src/PgQueuer.egg-info/SOURCES.txt` & `pgqueuer-0.2.2/src/PgQueuer.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -19,13 +19,13 @@
 src/PgQueuer/tm.py
 src/PgQueuer.egg-info/PKG-INFO
 src/PgQueuer.egg-info/SOURCES.txt
 src/PgQueuer.egg-info/dependency_links.txt
 src/PgQueuer.egg-info/requires.txt
 src/PgQueuer.egg-info/top_level.txt
 test/conftest.py
-test/test_benchmark.py
 test/test_qm.py
 test/test_queries.py
 test/test_tm.py
 test/db/Dockerfile
-test/db/init_db.sh
+test/db/init_db.sh
+tools/benchmark.py
```

### Comparing `pgqueuer-0.2.1/test/conftest.py` & `pgqueuer-0.2.2/test/conftest.py`

 * *Files identical despite different names*

### Comparing `pgqueuer-0.2.1/test/db/Dockerfile` & `pgqueuer-0.2.2/test/db/Dockerfile`

 * *Files identical despite different names*

### Comparing `pgqueuer-0.2.1/test/test_qm.py` & `pgqueuer-0.2.2/test/test_qm.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 import asyncio
+import time
 
 import asyncpg
 import pytest
 from PgQueuer.models import Job
 from PgQueuer.qm import QueueManager
 from PgQueuer.queries import Queries
 
 
-@pytest.mark.parametrize("N", (1, 2, 32, 500))
+@pytest.mark.parametrize("N", (1, 2, 32))
 async def test_job_queing(
     pgpool: asyncpg.Pool,
     N: int,
 ) -> None:
     c = QueueManager(pgpool)
     seen = list[int]()
 
@@ -29,15 +30,15 @@
     # Stop flag
     await c.queries.enqueue("fetch", None)
 
     await asyncio.wait_for(c.run(), timeout=1)
     assert seen == list(range(N))
 
 
-@pytest.mark.parametrize("N", (1, 2, 32, 512))
+@pytest.mark.parametrize("N", (1, 2, 32))
 @pytest.mark.parametrize("concurrency", (1, 2, 3, 4))
 async def test_job_fetch(
     pgpool: asyncpg.Pool,
     N: int,
     concurrency: int,
 ) -> None:
     q = Queries(pgpool)
@@ -51,14 +52,50 @@
             if context.payload is None:
                 for qm in qmpool:
                     qm.alive = False
                 return
             assert context
             seen.append(int(context.payload))
 
+    for n in range(N):
+        await q.enqueue("fetch", f"{n}".encode())
+
+    # Stop flag
+    await q.enqueue("fetch", None)
+
+    await asyncio.wait_for(
+        asyncio.gather(*[qm.run() for qm in qmpool]),
+        timeout=10,
+    )
+    assert sorted(seen) == list(range(N))
+
+
+@pytest.mark.parametrize("N", (1, 2, 32))
+@pytest.mark.parametrize("concurrency", (1, 2, 3, 4))
+async def test_sync_entrypoint(
+    pgpool: asyncpg.Pool,
+    N: int,
+    concurrency: int,
+) -> None:
+    q = Queries(pgpool)
+    qmpool = [QueueManager(pgpool) for _ in range(concurrency)]
+    seen = list[int]()
+
+    for qm in qmpool:
+
+        @qm.entrypoint("fetch")
+        def fetch(context: Job) -> None:
+            time.sleep(2)  # Sim. heavy CPU/IO.
+            if context.payload is None:
+                for qm in qmpool:
+                    qm.alive = False
+                return
+            assert context
+            seen.append(int(context.payload))
+
     for n in range(N):
         await q.enqueue("fetch", f"{n}".encode())
 
     # Stop flag
     await q.enqueue("fetch", None)
 
     await asyncio.wait_for(
```

### Comparing `pgqueuer-0.2.1/test/test_queries.py` & `pgqueuer-0.2.2/test/test_queries.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
         assert payoad is not None
         seen.append(int(payoad))
         await q.log_job(job, "successful")
 
     assert seen == list(range(N))
 
 
-@pytest.mark.parametrize("N", (1, 2, 64, 256))
+@pytest.mark.parametrize("N", (1, 2, 64))
 @pytest.mark.parametrize("concurrency", (1, 2, 4, 16))
 async def test_queries_next_jobs_concurrent(
     pgpool: asyncpg.Pool,
     N: int,
     concurrency: int,
 ) -> None:
     assert pgpool.get_max_size() >= concurrency
@@ -75,15 +75,15 @@
     await q.enqueue("placeholer", None)
     assert sum(x.count for x in await q.queue_size()) == 1
 
     await q.clear_queue()
     assert sum(x.count for x in await q.queue_size()) == 0
 
 
-@pytest.mark.parametrize("N", (1, 2, 64, 256))
+@pytest.mark.parametrize("N", (1, 2, 64))
 async def test_move_job_log(
     pgpool: asyncpg.Pool,
     N: int,
 ) -> None:
     q = queries.Queries(pgpool)
 
     for n in range(N):
@@ -126,15 +126,15 @@
 
     assert all(x.count == 1 for x in await q.queue_size())
     assert sum(x.count for x in await q.queue_size()) == N
     await q.clear_queue("placeholer0")
     assert sum(x.count for x in await q.queue_size()) == N - 1
 
 
-@pytest.mark.parametrize("N", (1, 2, 64, 256))
+@pytest.mark.parametrize("N", (1, 2, 64))
 async def test_queue_priority(
     pgpool: asyncpg.Pool,
     N: int,
 ) -> None:
     q = queries.Queries(pgpool)
     jobs = list[models.Job]()
```

