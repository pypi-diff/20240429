# Comparing `tmp/starlette_testclient-0.3.0.tar.gz` & `tmp/starlette_testclient-0.4.0.tar.gz`

## Comparing `starlette_testclient-0.3.0.tar` & `starlette_testclient-0.4.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 starlette_testclient-0.3.0/.cruft.json
--rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 starlette_testclient-0.3.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 starlette_testclient-0.3.0/requirements.txt
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 starlette_testclient-0.3.0/setup.py
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 starlette_testclient-0.3.0/.github/dependabot.yml
--rw-r--r--   0        0        0      923 2020-02-02 00:00:00.000000 starlette_testclient-0.3.0/.github/workflows/main.yml
--rw-r--r--   0        0        0     1378 2020-02-02 00:00:00.000000 starlette_testclient-0.3.0/.github/workflows/publish.yml
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 starlette_testclient-0.3.0/starlette_testclient/__init__.py
--rw-r--r--   0        0        0    19656 2020-02-02 00:00:00.000000 starlette_testclient-0.3.0/starlette_testclient/_testclient.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 starlette_testclient-0.3.0/starlette_testclient/py.typed
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 starlette_testclient-0.3.0/tests/__init__.py
--rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 starlette_testclient-0.3.0/tests/conftest.py
--rw-r--r--   0        0        0     7398 2020-02-02 00:00:00.000000 starlette_testclient-0.3.0/tests/test_testclient.py
--rw-r--r--   0        0        0     2035 2020-02-02 00:00:00.000000 starlette_testclient-0.3.0/.gitignore
--rw-r--r--   0        0        0     1557 2020-02-02 00:00:00.000000 starlette_testclient-0.3.0/LICENSE
--rw-r--r--   0        0        0     1247 2020-02-02 00:00:00.000000 starlette_testclient-0.3.0/README.md
--rw-r--r--   0        0        0     2108 2020-02-02 00:00:00.000000 starlette_testclient-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     2445 2020-02-02 00:00:00.000000 starlette_testclient-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 starlette_testclient-0.4.0/.cruft.json
+-rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 starlette_testclient-0.4.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 starlette_testclient-0.4.0/requirements.txt
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 starlette_testclient-0.4.0/setup.py
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 starlette_testclient-0.4.0/.github/dependabot.yml
+-rw-r--r--   0        0        0     1246 2020-02-02 00:00:00.000000 starlette_testclient-0.4.0/.github/workflows/main.yml
+-rw-r--r--   0        0        0     1378 2020-02-02 00:00:00.000000 starlette_testclient-0.4.0/.github/workflows/publish.yml
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 starlette_testclient-0.4.0/starlette_testclient/__init__.py
+-rw-r--r--   0        0        0    19816 2020-02-02 00:00:00.000000 starlette_testclient-0.4.0/starlette_testclient/_testclient.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 starlette_testclient-0.4.0/starlette_testclient/py.typed
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 starlette_testclient-0.4.0/tests/__init__.py
+-rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 starlette_testclient-0.4.0/tests/conftest.py
+-rw-r--r--   0        0        0     7432 2020-02-02 00:00:00.000000 starlette_testclient-0.4.0/tests/test_testclient.py
+-rw-r--r--   0        0        0     2035 2020-02-02 00:00:00.000000 starlette_testclient-0.4.0/.gitignore
+-rw-r--r--   0        0        0     1557 2020-02-02 00:00:00.000000 starlette_testclient-0.4.0/LICENSE
+-rw-r--r--   0        0        0     1247 2020-02-02 00:00:00.000000 starlette_testclient-0.4.0/README.md
+-rw-r--r--   0        0        0     2154 2020-02-02 00:00:00.000000 starlette_testclient-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     2496 2020-02-02 00:00:00.000000 starlette_testclient-0.4.0/PKG-INFO
```

### Comparing `starlette_testclient-0.3.0/.cruft.json` & `starlette_testclient-0.4.0/.cruft.json`

 * *Files identical despite different names*

### Comparing `starlette_testclient-0.3.0/.pre-commit-config.yaml` & `starlette_testclient-0.4.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `starlette_testclient-0.3.0/setup.py` & `starlette_testclient-0.4.0/setup.py`

 * *Files identical despite different names*

### Comparing `starlette_testclient-0.3.0/.github/workflows/main.yml` & `starlette_testclient-0.4.0/.github/workflows/main.yml`

 * *Files 23% similar despite different names*

```diff
@@ -10,15 +10,15 @@
   tests:
     name: "Python ${{ matrix.python-version }}"
     runs-on: ubuntu-latest
 
     timeout-minutes: 30
     strategy:
       matrix:
-        python-version: ["3.7", "3.8", "3.9", "3.10", "3.11"]
+        python-version: ["3.7", "3.8", "3.9", "3.10", "3.11", "3.12"]
 
     steps:
       - uses: actions/checkout@v3
       - uses: actions/setup-python@v3
         with:
           python-version: ${{ matrix.python-version }}
 
@@ -32,9 +32,21 @@
           key: pip-${{ matrix.python-version }}
 
       - name: Install dependencies
         run: |
           python -m pip install --upgrade pip setuptools wheel
           python -m pip install -r requirements.txt
 
+      - name: Downgrade trio
+        if: ${{ matrix.python-version == '3.7' }}
+        run: |
+          python -m pip install "trio==0.21"
+
       - name: Run tests
         run: python -m coverage run -m pytest
+
+      - name: Downgrade anyio
+        run: |
+          python -m pip install "anyio<4" "trio==0.21"
+
+      - name: Re-run tests
+        run: python -m coverage run -m pytest
```

### Comparing `starlette_testclient-0.3.0/.github/workflows/publish.yml` & `starlette_testclient-0.4.0/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `starlette_testclient-0.3.0/starlette_testclient/_testclient.py` & `starlette_testclient-0.4.0/starlette_testclient/_testclient.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,14 +20,18 @@
 from starlette.websockets import WebSocketDisconnect
 
 if sys.version_info >= (3, 8):  # pragma: no cover
     from typing import TypedDict
 else:  # pragma: no cover
     from typing_extensions import TypedDict
 
+try:
+    start_blocking_portal = anyio.from_thread.start_blocking_portal
+except AttributeError:  # pragma: no cover
+    start_blocking_portal = anyio.start_blocking_portal
 
 _PortalFactoryType = typing.Callable[
     [], typing.ContextManager[anyio.abc.BlockingPortal]
 ]
 
 
 # Annotations for `Session.request()`
@@ -443,15 +447,15 @@
     @contextlib.contextmanager
     def _portal_factory(
         self,
     ) -> typing.Generator[anyio.abc.BlockingPortal, None, None]:
         if self.portal is not None:
             yield self.portal
         else:
-            with anyio.start_blocking_portal(**self.async_backend) as portal:
+            with start_blocking_portal(**self.async_backend) as portal:
                 yield portal
 
     def request(  # type: ignore
         self,
         method: str,
         url: str,
         params: Params = None,
@@ -508,15 +512,15 @@
             raise RuntimeError("Expected WebSocket upgrade")  # pragma: no cover
 
         return session
 
     def __enter__(self) -> "TestClient":
         with contextlib.ExitStack() as stack:
             self.portal = portal = stack.enter_context(
-                anyio.start_blocking_portal(**self.async_backend)
+                start_blocking_portal(**self.async_backend)
             )
 
             @stack.callback
             def reset_portal() -> None:
                 self.portal = None
 
             self.stream_send = StapledObjectStream(
```

### Comparing `starlette_testclient-0.3.0/tests/test_testclient.py` & `starlette_testclient-0.4.0/tests/test_testclient.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,19 +35,20 @@
         task = asyncio_current_task()
         if task is None:
             raise RuntimeError("must be called from a running task")  # pragma: no cover
         return task
     raise RuntimeError(f"unsupported asynclib={asynclib_name}")  # pragma: no cover
 
 
-def startup():
+@asynccontextmanager
+def lifespan(*args, **kwargs):
     raise RuntimeError()
 
 
-startup_error_app = Starlette(on_startup=[startup])
+startup_error_app = Starlette(lifespan=lifespan)
 
 
 def test_use_testclient_in_endpoint(test_client_factory):
     """
     We should be able to use the test client within applications.
 
     This is useful if we need to mock out other services,
```

### Comparing `starlette_testclient-0.3.0/.gitignore` & `starlette_testclient-0.4.0/.gitignore`

 * *Files identical despite different names*

### Comparing `starlette_testclient-0.3.0/LICENSE` & `starlette_testclient-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `starlette_testclient-0.3.0/README.md` & `starlette_testclient-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `starlette_testclient-0.3.0/pyproject.toml` & `starlette_testclient-0.4.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = 'hatchling.build'
 
 [project]
 name = "starlette-testclient"
-version = "0.3.0"
+version = "0.4.0"
 description = "A backport of Starlette TestClient using requests! ⏪️"
 readme = "README.md"
 authors = [{ name = "Marcelo Trylesinski", email = "marcelotryle@email.com" }]
 classifiers = [
     "Development Status :: 3 - Alpha",
     "License :: OSI Approved :: BSD License",
     "Intended Audience :: Developers",
@@ -17,14 +17,15 @@
     "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
 ]
 license = "BSD-3-Clause"
 requires-python = ">=3.7"
 dependencies = [
     "starlette >= 0.20.1",
     "requests",
 ]
```

### Comparing `starlette_testclient-0.3.0/PKG-INFO` & `starlette_testclient-0.4.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: starlette-testclient
-Version: 0.3.0
+Version: 0.4.0
 Summary: A backport of Starlette TestClient using requests! ⏪️
 Project-URL: Homepage, https://github.com/Kludex/starlette-testclient
 Project-URL: Source, https://github.com/Kludex/starlette-testclient
 Project-URL: Twitter, https://twitter.com/marcelotryle
 Project-URL: Funding, https://github.com/sponsors/Kludex
 Author-email: Marcelo Trylesinski <marcelotryle@email.com>
 License-Expression: BSD-3-Clause
@@ -17,14 +17,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.7
 Requires-Dist: requests
 Requires-Dist: starlette>=0.20.1
 Description-Content-Type: text/markdown
 
 <h1 align="center">
     <strong>starlette-testclient</strong>
```

#### html2text {}

```diff
@@ -1,24 +1,24 @@
-Metadata-Version: 2.1 Name: starlette-testclient Version: 0.3.0 Summary: A
+Metadata-Version: 2.3 Name: starlette-testclient Version: 0.4.0 Summary: A
 backport of Starlette TestClient using requests! âªï¸ Project-URL: Homepage,
 https://github.com/Kludex/starlette-testclient Project-URL: Source, https://
 github.com/Kludex/starlette-testclient Project-URL: Twitter, https://
 twitter.com/marcelotryle Project-URL: Funding, https://github.com/sponsors/
 Kludex Author-email: Marcelo Trylesinski
 email.com> License-Expression: BSD-3-Clause License-File: LICENSE Classifier:
 Development Status :: 3 - Alpha Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License Classifier: Natural Language
 :: English Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3 :: Only Classifier: Programming Language :: Python :: 3.7 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
 Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
-Programming Language :: Python :: 3.11 Requires-Python: >=3.7 Requires-Dist:
-requests Requires-Dist: starlette>=0.20.1 Description-Content-Type: text/
-markdown
+Programming Language :: Python :: 3.11 Classifier: Programming Language ::
+Python :: 3.12 Requires-Python: >=3.7 Requires-Dist: requests Requires-Dist:
+starlette>=0.20.1 Description-Content-Type: text/markdown
                       ************ ssttaarrlleettttee--tteessttcclliieenntt ************
 _[_L_a_t_e_s_t_ _C_o_m_m_i_t_][https://img.shields.io/github/workflow/status/Kludex/starlette-
                                 testclient/CI]
 _[_P_a_c_k_a_g_e_ _v_e_r_s_i_o_n_][https://img.shields.io/pypi/pyversions/starlette-testclient]
       [https://img.shields.io/github/license/Kludex/starlette-testclient]
 This is a backport of Starlette's `TestClient` using `requests` instead of
 `httpx`. The reason behind here is to give more time for people to migrate. ##
```

