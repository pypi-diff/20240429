# Comparing `tmp/vaping-1.5.3.tar.gz` & `tmp/vaping-1.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vaping-1.5.3.tar", max compression
+gzip compressed data, was "vaping-1.5.4.tar", max compression
```

## Comparing `vaping-1.5.3.tar` & `vaping-1.5.4.tar`

### file list

```diff
@@ -1,23 +1,22 @@
--rw-r--r--   0        0        0    11358 2022-08-11 15:47:40.405766 vaping-1.5.3/LICENSE
--rw-r--r--   0        0        0     3881 2022-08-11 16:09:09.534601 vaping-1.5.3/README.md
--rw-r--r--   0        0        0     2714 2022-09-02 08:04:48.617119 vaping-1.5.3/pyproject.toml
--rw-r--r--   0        0        0     1143 2022-08-11 15:47:40.415766 vaping-1.5.3/src/vaping/__init__.py
--rw-r--r--   0        0        0     4666 2022-08-11 15:47:40.415766 vaping-1.5.3/src/vaping/asyncio_backport.py
--rw-r--r--   0        0        0     2116 2022-08-11 15:47:40.415766 vaping-1.5.3/src/vaping/cli.py
--rw-r--r--   0        0        0     1148 2022-08-11 15:47:40.415766 vaping-1.5.3/src/vaping/config/__init__.py
--rw-r--r--   0        0        0     2479 2022-08-11 15:47:40.415766 vaping-1.5.3/src/vaping/config/schema.py
--rw-r--r--   0        0        0     7697 2022-08-11 15:47:40.415766 vaping-1.5.3/src/vaping/daemon.py
--rw-r--r--   0        0        0      649 2022-08-11 15:47:40.415766 vaping-1.5.3/src/vaping/io.py
--rw-r--r--   0        0        0    16356 2022-08-11 15:47:40.415766 vaping-1.5.3/src/vaping/plugins/__init__.py
--rw-r--r--   0        0        0     1622 2022-08-11 15:47:40.415766 vaping-1.5.3/src/vaping/plugins/command.py
--rw-r--r--   0        0        0     5100 2022-08-11 15:47:40.415766 vaping-1.5.3/src/vaping/plugins/fping.py
--rw-r--r--   0        0        0     3239 2022-08-11 15:47:40.415766 vaping-1.5.3/src/vaping/plugins/fping_mtr.py
--rw-r--r--   0        0        0     2364 2022-08-11 15:47:40.415766 vaping-1.5.3/src/vaping/plugins/graphite.py
--rw-r--r--   0        0        0    12706 2022-08-11 15:47:40.415766 vaping-1.5.3/src/vaping/plugins/logparse.py
--rw-r--r--   0        0        0     1616 2022-08-11 15:47:40.415766 vaping-1.5.3/src/vaping/plugins/prometheus.py
--rw-r--r--   0        0        0     1397 2022-08-11 15:47:40.415766 vaping-1.5.3/src/vaping/plugins/rrd.py
--rw-r--r--   0        0        0     3075 2022-08-11 15:47:40.415766 vaping-1.5.3/src/vaping/plugins/vodka.py
--rw-r--r--   0        0        0     1968 2022-08-11 15:47:40.415766 vaping-1.5.3/src/vaping/plugins/whisper.py
--rw-r--r--   0        0        0     1805 2022-08-11 15:47:40.415766 vaping-1.5.3/src/vaping/plugins/zeromq.py
--rw-r--r--   0        0        0     5518 2022-09-02 08:05:02.010142 vaping-1.5.3/setup.py
--rw-r--r--   0        0        0     5993 2022-09-02 08:05:02.012052 vaping-1.5.3/PKG-INFO
+-rw-r--r--   0        0        0    11358 2020-07-26 07:03:13.893474 vaping-1.5.4/LICENSE
+-rw-r--r--   0        0        0     3899 2024-04-28 01:52:36.448661 vaping-1.5.4/README.md
+-rw-r--r--   0        0        0     2674 2024-04-29 02:19:38.376191 vaping-1.5.4/pyproject.toml
+-rw-r--r--   0        0        0     1143 2021-05-28 01:14:36.120985 vaping-1.5.4/src/vaping/__init__.py
+-rw-r--r--   0        0        0     4666 2021-07-17 15:55:56.281366 vaping-1.5.4/src/vaping/asyncio_backport.py
+-rw-r--r--   0        0        0     2116 2021-05-28 01:14:36.121986 vaping-1.5.4/src/vaping/cli.py
+-rw-r--r--   0        0        0     1148 2021-05-28 01:14:36.121986 vaping-1.5.4/src/vaping/config/__init__.py
+-rw-r--r--   0        0        0     2455 2024-04-29 02:15:20.720777 vaping-1.5.4/src/vaping/config/schema.py
+-rw-r--r--   0        0        0     7697 2022-03-21 11:39:06.197034 vaping-1.5.4/src/vaping/daemon.py
+-rw-r--r--   0        0        0      649 2021-07-17 15:55:56.282366 vaping-1.5.4/src/vaping/io.py
+-rw-r--r--   0        0        0    16353 2024-04-28 01:52:36.450661 vaping-1.5.4/src/vaping/plugins/__init__.py
+-rw-r--r--   0        0        0     1622 2021-05-28 01:14:36.122985 vaping-1.5.4/src/vaping/plugins/command.py
+-rw-r--r--   0        0        0     5100 2022-03-21 11:39:06.198034 vaping-1.5.4/src/vaping/plugins/fping.py
+-rw-r--r--   0        0        0     3239 2022-03-21 11:39:06.199034 vaping-1.5.4/src/vaping/plugins/fping_mtr.py
+-rw-r--r--   0        0        0     2363 2024-04-28 01:52:36.450661 vaping-1.5.4/src/vaping/plugins/graphite.py
+-rw-r--r--   0        0        0    12704 2024-04-28 01:52:36.450661 vaping-1.5.4/src/vaping/plugins/logparse.py
+-rw-r--r--   0        0        0     1615 2024-04-28 01:52:36.450661 vaping-1.5.4/src/vaping/plugins/prometheus.py
+-rw-r--r--   0        0        0     1397 2021-07-17 15:55:56.284366 vaping-1.5.4/src/vaping/plugins/rrd.py
+-rw-r--r--   0        0        0     3074 2024-04-28 01:52:36.450661 vaping-1.5.4/src/vaping/plugins/vodka.py
+-rw-r--r--   0        0        0     1968 2021-07-17 15:55:56.284366 vaping-1.5.4/src/vaping/plugins/whisper.py
+-rw-r--r--   0        0        0     1805 2022-03-21 11:39:06.199034 vaping-1.5.4/src/vaping/plugins/zeromq.py
+-rw-r--r--   0        0        0     6063 1970-01-01 00:00:00.000000 vaping-1.5.4/PKG-INFO
```

### Comparing `vaping-1.5.3/LICENSE` & `vaping-1.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `vaping-1.5.3/README.md` & `vaping-1.5.4/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 
 # Vaping
 
 [![PyPI](https://img.shields.io/pypi/v/vaping.svg?maxAge=60)](https://pypi.python.org/pypi/vaping)
 [![PyPI](https://img.shields.io/pypi/pyversions/vaping.svg?maxAge=600)](https://pypi.python.org/pypi/vaping)
 [![Tests](https://github.com/20c/vaping/workflows/tests/badge.svg)](https://github.com/20c/vaping)
-[![LGTM Grade](https://img.shields.io/lgtm/grade/python/github/20c/vaping)](https://lgtm.com/projects/g/20c/vaping/alerts/)
+[![CodeQL](https://github.com/20c/vaping/actions/workflows/codeql.yml/badge.svg)](https://github.com/20c/vaping/actions/workflows/codeql.yml)
 [![Codecov](https://img.shields.io/codecov/c/github/20c/vaping/master.svg)](https://codecov.io/github/20c/vaping)
 
 
 vaping is a healthy alternative to smokeping!*
 
 * (This statement has not been evaluated by the Food and Drug Administration)
```

### Comparing `vaping-1.5.3/pyproject.toml` & `vaping-1.5.4/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,57 +1,59 @@
 [tool.poetry]
 name = "vaping"
-version = "1.5.3"
+version = "1.5.4"
 description = "vaping is a healthy alternative to smokeping!"
 readme = "README.md"
 repository = "https://github.com/20c/vaping"
 authors = ["20C <code@20c.com>"]
 license = "Apache-2.0"
 
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     'Environment :: No Input/Output (Daemon)',
     'Intended Audience :: System Administrators',
     'Intended Audience :: Telecommunications Industry',
     'License :: OSI Approved :: Apache Software License',
-    'Programming Language :: Python :: 3.7',
     'Programming Language :: Python :: 3.8',
     'Programming Language :: Python :: 3.9',
     'Programming Language :: Python :: 3.10',
+    'Programming Language :: Python :: 3.11',
     'Topic :: Internet',
     'Topic :: Software Development :: Libraries :: Python Modules',
     'Topic :: System :: Monitoring',
     'Topic :: System :: Networking :: Monitoring',
 ]
 
 packages = [{ include = "vaping", from = "src" }]
 
 [tool.poetry.scripts]
 vaping = "vaping.cli:cli"
 
 
 [tool.poetry.dependencies]
-python = "^3.7"
-pid = "^3"
-pluginmgr = "^1"
-python-daemon = "^2"
-munge = { extras = ["tomlkit", "yaml"], version = "^1.2.0" }
-confu = "^1.7.1"
+python = "^3.8"
+pid = ">=3"
+pluginmgr = ">=1.2"
+python-daemon = ">=2"
+# Package docutils (0.21.post1) not found.
+docutils = "<=0.21"
+munge = { extras = ["tomlkit", "yaml"], version = ">=1.2.0" }
+confu = ">=1.7.1"
 
 # plugins
 
 # graphite
-requests = { version = "^2.19.1", optional = true }
-graphyte = { version = "^1.4", optional = true }
+requests = { version = ">=2.19.1", optional = true }
+graphyte = { version = ">=1.4", optional = true }
 
 # rrdtool
 rrdtool = { version = ">=0.1.14, <1", optional = true }
 
 # prometheus
-prometheus_client = { version = "^0.11.0", optional = true }
+prometheus_client = { version = ">=0.11.0", optional = true }
 
 # standalone
 graphsrv = { version = "^2", optional = true }
 vodka = { version = "^3.1", optional = true }
 # FIXME: wekzeug >2.1.0 breaks static file serving
 Werkzeug = { version = ">2,<2.1.0", optional = true }
 Flask = { version = ">2,<2.2", optional = true }
@@ -60,40 +62,36 @@
 whisper = { version = ">=0.9.15, <2", optional = true }
 
 # zeromq
 pyzmq = { version = ">=15.3.0", optional = true }
 
 [tool.poetry.dev-dependencies]
 # tests
-codecov = "^2.1.10"
-coverage = "^5.3"
-pytest = "^6.1.2"
-pytest-cov = "^2.10.1"
-pytest-filedata = "^0.4.0"
-tox = "^3.20.1"
+coverage = ">=5.3"
+pytest = ">=6.1.2"
+pytest-cov = ">=2.10.1"
+pytest-filedata = ">=1"
+tox = ">=3.20.1"
 
 # linting
-# bandit = "^1.6.2"
-black = ">=20"
-isort = "^5.7.0"
-flake8 = "^3.8.4"
-pre-commit = "^2.13"
-pyupgrade = "^2.19.4"
-mypy = "^0.812"
+ruff = ">=0.1"
+mypy = ">=0.950"
+pre-commit = ">=2.13"
+pyupgrade = ">=2.19"
 
 # ctl
-ctl = "^1"
-jinja2 = "^3"
-tmpl = "^1"
-twine = "^3.3.0"
+ctl = ">=1"
+jinja2 = ">=3"
+tmpl = ">=1"
+twine = ">=3.3.0"
 
 # docs
 markdown-include = ">=0.5,<1"
-mkdocs = "^1.2.3"
-pymdgen = "^1"
+mkdocs = ">=1.2.3"
+pymdgen = ">=1"
 
 [tool.poetry.extras]
 graphite = ["graphyte", "requests"]
 rrdtool = ["rrdtool"]
 prometheus = ["prometheus_client"]
 standalone = ["graphsrv", "vodka"]
 whisper = ["whisper"]
@@ -107,14 +105,10 @@
     "pyzmq",
     "rrdtool",
     "requests",
     "vodka",
     "whisper",
 ]
 
-[tool.isort]
-profile = "black"
-multi_line_output = 3
-
 [build-system]
-requires = ["poetry>=0.12"]
-build-backend = "poetry.masonry.api"
+requires = ["poetry-core>=1"]
+build-backend = "poetry.core.masonry.api"
```

### Comparing `vaping-1.5.3/src/vaping/__init__.py` & `vaping-1.5.4/src/vaping/__init__.py`

 * *Files identical despite different names*

### Comparing `vaping-1.5.3/src/vaping/asyncio_backport.py` & `vaping-1.5.4/src/vaping/asyncio_backport.py`

 * *Files identical despite different names*

### Comparing `vaping-1.5.3/src/vaping/cli.py` & `vaping-1.5.4/src/vaping/cli.py`

 * *Files identical despite different names*

### Comparing `vaping-1.5.3/src/vaping/config/__init__.py` & `vaping-1.5.4/src/vaping/config/__init__.py`

 * *Files identical despite different names*

### Comparing `vaping-1.5.3/src/vaping/config/schema.py` & `vaping-1.5.4/src/vaping/config/schema.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import confu.exceptions
 import confu.generator
 import confu.schema
 
 
 class MixedDict(confu.schema.Dict):
     """
     Extended confu.schema.Dict object that prevents
```

### Comparing `vaping-1.5.3/src/vaping/daemon.py` & `vaping-1.5.4/src/vaping/daemon.py`

 * *Files identical despite different names*

### Comparing `vaping-1.5.3/src/vaping/io.py` & `vaping-1.5.4/src/vaping/io.py`

 * *Files identical despite different names*

### Comparing `vaping-1.5.3/src/vaping/plugins/__init__.py` & `vaping-1.5.4/src/vaping/plugins/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,15 +53,14 @@
     lazy_start = False
 
     ConfigSchema = PluginConfigSchema
     ConfigSchema.help = "Base plugin config schema"
 
     @property
     def groups(self):
-
         """
         `dict` - group configurations keyed by name
         """
 
         group_config = {}
 
         # legacy way of threating any dict as a potential
@@ -270,15 +269,14 @@
             raise ValueError("interval not set in config")
         self.interval = parse_interval(self.pluginmgr_config["interval"])
         self.run_level = 0
 
     async def _run(self):
         self.run_level = 1
         while self.run_level:
-
             start = datetime.datetime.now()
 
             # since the TimedProbe will sleep between cycles
             # we need to emit all queued emissions each cycle
             await self.emit_all()
 
             msg = self.probe()
@@ -571,15 +569,14 @@
         **Arguments**
 
         - message (`dict`): vaping message dict
         """
         # handle vaping data that arrives in a list
         if isinstance(message.get("data"), list):
             for row in message.get("data"):
-
                 if row is None:
                     self.log.debug(
                         "Ignoring empty row from {}/{}".format(
                             message.get("source"), message.get("type")
                         )
                     )
                     continue
```

### Comparing `vaping-1.5.3/src/vaping/plugins/command.py` & `vaping-1.5.4/src/vaping/plugins/command.py`

 * *Files identical despite different names*

### Comparing `vaping-1.5.3/src/vaping/plugins/fping.py` & `vaping-1.5.4/src/vaping/plugins/fping.py`

 * *Files identical despite different names*

### Comparing `vaping-1.5.3/src/vaping/plugins/fping_mtr.py` & `vaping-1.5.4/src/vaping/plugins/fping_mtr.py`

 * *Files identical despite different names*

### Comparing `vaping-1.5.3/src/vaping/plugins/graphite.py` & `vaping-1.5.4/src/vaping/plugins/graphite.py`

 * *Files 0% similar despite different names*

```diff
@@ -54,15 +54,14 @@
     def start(self):
         graphyte.init(str(self.graphite_host), prefix=str(self.prefix))
 
     def create(self, filename):
         return
 
     def update(self, filename, time, value):
-
         if value is None:
             return
 
         filename = munge_filename(filename)
         graphyte.send(f"{filename}", value, time)
 
     def get(self, filename, from_time, to_time=None):
```

### Comparing `vaping-1.5.3/src/vaping/plugins/logparse.py` & `vaping-1.5.4/src/vaping/plugins/logparse.py`

 * *Files 0% similar despite different names*

```diff
@@ -211,15 +211,14 @@
         **Returns**
 
         seconds (`float`)
         """
         return vaping.config.parse_interval(value)
 
     def aggregate(self, messages):
-
         """
         Takes a list of messages and aggregates them
         according to aggration config
 
         **Arguments**
 
         - messagges (`list<dict>`)
@@ -243,15 +242,14 @@
         # return empty list
         if len(self.stack) < self.aggregate_count:
             return rv
 
         # while stack is bigger than the aggregation count
         # pop messages off the stack and aggregate
         while len(self.stack) >= self.aggregate_count:
-
             # pop first message in stack
             message = self.stack[0]
             self.stack.remove(self.stack[0])
 
             # join data of other messages to first message
             # no aggregation yet
             for other in self.stack[: self.aggregate_count - 1]:
```

### Comparing `vaping-1.5.3/src/vaping/plugins/prometheus.py` & `vaping-1.5.4/src/vaping/plugins/prometheus.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,14 @@
         start_http_server(port)
 
     def emit(self, data):
         raw_data = data.get("data")
 
         self.log.debug("data: " + str(raw_data))
         for host_data in raw_data:
-
             if host_data is None:
                 continue
 
             host_name = host_data.get("host")
             if "min" in host_data:
                 min_latency.labels(host_name).observe(host_data.get("min"))
             if "max" in host_data:
```

### Comparing `vaping-1.5.3/src/vaping/plugins/rrd.py` & `vaping-1.5.4/src/vaping/plugins/rrd.py`

 * *Files identical despite different names*

### Comparing `vaping-1.5.3/src/vaping/plugins/vodka.py` & `vaping-1.5.4/src/vaping/plugins/vodka.py`

 * *Files 0% similar despite different names*

```diff
@@ -82,15 +82,14 @@
     # Define config schema
     ConfigSchema = VodkaSchema
 
     def init(self):
         self._is_started = False
 
     def start(self):
-
         if self._is_started:
             return
 
         # deep copy vodka plugin config and prepare to pass
         # to vodka as it's own copy with type and name keys
         # removed
```

### Comparing `vaping-1.5.3/src/vaping/plugins/whisper.py` & `vaping-1.5.4/src/vaping/plugins/whisper.py`

 * *Files identical despite different names*

### Comparing `vaping-1.5.3/src/vaping/plugins/zeromq.py` & `vaping-1.5.4/src/vaping/plugins/zeromq.py`

 * *Files identical despite different names*

### Comparing `vaping-1.5.3/PKG-INFO` & `vaping-1.5.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,62 +1,64 @@
 Metadata-Version: 2.1
 Name: vaping
-Version: 1.5.3
+Version: 1.5.4
 Summary: vaping is a healthy alternative to smokeping!
 Home-page: https://github.com/20c/vaping
 License: Apache-2.0
 Author: 20C
 Author-email: code@20c.com
-Requires-Python: >=3.7,<4.0
+Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: No Input/Output (Daemon)
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Telecommunications Industry
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Internet
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: System :: Monitoring
 Classifier: Topic :: System :: Networking :: Monitoring
 Provides-Extra: all
 Provides-Extra: graphite
 Provides-Extra: prometheus
 Provides-Extra: rrdtool
 Provides-Extra: standalone
 Provides-Extra: whisper
 Provides-Extra: zeromq
 Requires-Dist: Flask (>2,<2.2)
 Requires-Dist: Werkzeug (>2,<2.1.0)
-Requires-Dist: confu (>=1.7.1,<2.0.0)
-Requires-Dist: graphsrv (>=2,<3); extra == "standalone" or extra == "all"
-Requires-Dist: graphyte (>=1.4,<2.0); extra == "graphite" or extra == "all"
-Requires-Dist: munge[yaml,tomlkit] (>=1.2.0,<2.0.0)
-Requires-Dist: pid (>=3,<4)
-Requires-Dist: pluginmgr (>=1,<2)
-Requires-Dist: prometheus_client (>=0.11.0,<0.12.0); extra == "prometheus" or extra == "all"
-Requires-Dist: python-daemon (>=2,<3)
-Requires-Dist: pyzmq (>=15.3.0); extra == "zeromq" or extra == "all"
-Requires-Dist: requests (>=2.19.1,<3.0.0); extra == "graphite" or extra == "all"
-Requires-Dist: rrdtool (>=0.1.14,<1); extra == "rrdtool" or extra == "all"
-Requires-Dist: vodka (>=3.1,<4.0); extra == "standalone" or extra == "all"
-Requires-Dist: whisper (>=0.9.15,<2); extra == "whisper" or extra == "all"
+Requires-Dist: confu (>=1.7.1)
+Requires-Dist: docutils (<=0.21)
+Requires-Dist: graphsrv (>=2,<3) ; extra == "standalone" or extra == "all"
+Requires-Dist: graphyte (>=1.4) ; extra == "graphite" or extra == "all"
+Requires-Dist: munge[tomlkit,yaml] (>=1.2.0)
+Requires-Dist: pid (>=3)
+Requires-Dist: pluginmgr (>=1.2)
+Requires-Dist: prometheus_client (>=0.11.0) ; extra == "prometheus" or extra == "all"
+Requires-Dist: python-daemon (>=2)
+Requires-Dist: pyzmq (>=15.3.0) ; extra == "zeromq" or extra == "all"
+Requires-Dist: requests (>=2.19.1) ; extra == "graphite" or extra == "all"
+Requires-Dist: rrdtool (>=0.1.14,<1) ; extra == "rrdtool" or extra == "all"
+Requires-Dist: vodka (>=3.1,<4.0) ; extra == "standalone" or extra == "all"
+Requires-Dist: whisper (>=0.9.15,<2) ; extra == "whisper" or extra == "all"
 Project-URL: Repository, https://github.com/20c/vaping
 Description-Content-Type: text/markdown
 
 
 # Vaping
 
 [![PyPI](https://img.shields.io/pypi/v/vaping.svg?maxAge=60)](https://pypi.python.org/pypi/vaping)
 [![PyPI](https://img.shields.io/pypi/pyversions/vaping.svg?maxAge=600)](https://pypi.python.org/pypi/vaping)
 [![Tests](https://github.com/20c/vaping/workflows/tests/badge.svg)](https://github.com/20c/vaping)
-[![LGTM Grade](https://img.shields.io/lgtm/grade/python/github/20c/vaping)](https://lgtm.com/projects/g/20c/vaping/alerts/)
+[![CodeQL](https://github.com/20c/vaping/actions/workflows/codeql.yml/badge.svg)](https://github.com/20c/vaping/actions/workflows/codeql.yml)
 [![Codecov](https://img.shields.io/codecov/c/github/20c/vaping/master.svg)](https://codecov.io/github/20c/vaping)
 
 
 vaping is a healthy alternative to smokeping!*
 
 * (This statement has not been evaluated by the Food and Drug Administration)
```

