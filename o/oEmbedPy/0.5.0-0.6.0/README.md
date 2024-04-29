# Comparing `tmp/oembedpy-0.5.0.tar.gz` & `tmp/oembedpy-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oembedpy-0.5.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "oembedpy-0.6.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `oembedpy-0.5.0.tar` & `oembedpy-0.6.0.tar`

### file list

```diff
@@ -1,38 +1,40 @@
--rw-r--r--   0        0        0      861 2024-04-21 05:40:56.126496 oembedpy-0.5.0/.age.toml
--rw-r--r--   0        0        0      560 2024-04-21 05:40:56.126496 oembedpy-0.5.0/.editorconfig
--rw-r--r--   0        0        0      159 2024-04-21 05:40:56.126496 oembedpy-0.5.0/.github/release-body.md
--rw-r--r--   0        0        0     1784 2024-04-21 05:40:56.126496 oembedpy-0.5.0/.github/workflows/main.yml
--rwxr-xr-x   0        0        0     2695 2024-04-21 05:40:56.126496 oembedpy-0.5.0/.github/workflows/release.yml
--rw-r--r--   0        0        0     3338 2024-04-21 05:40:56.126496 oembedpy-0.5.0/.gitignore
--rw-r--r--   0        0        0      333 2024-04-21 05:40:56.126496 oembedpy-0.5.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      500 2024-04-21 05:40:56.126496 oembedpy-0.5.0/.readthedocs.yml
--rw-r--r--   0        0        0     1967 2024-04-21 05:40:56.126496 oembedpy-0.5.0/CHANGES.rst
--rw-r--r--   0        0        0     9161 2024-04-21 05:40:56.126496 oembedpy-0.5.0/LICENSE
--rw-r--r--   0        0        0     1299 2024-04-21 05:40:56.126496 oembedpy-0.5.0/README.rst
--rw-r--r--   0        0        0        5 2024-04-21 05:40:56.126496 oembedpy-0.5.0/docs/.gitignore
--rw-r--r--   0        0        0      699 2024-04-21 05:40:56.126496 oembedpy-0.5.0/docs/Makefile
--rw-r--r--   0        0        0       89 2024-04-21 05:40:56.126496 oembedpy-0.5.0/docs/api.rst
--rw-r--r--   0        0        0      211 2024-04-21 05:40:56.126496 oembedpy-0.5.0/docs/changelogs.rst
--rw-r--r--   0        0        0      461 2024-04-21 05:40:56.126496 oembedpy-0.5.0/docs/commandline.rst
--rw-r--r--   0        0        0      302 2024-04-21 05:40:56.126496 oembedpy-0.5.0/docs/conf.py
--rw-r--r--   0        0        0      377 2024-04-21 05:40:56.126496 oembedpy-0.5.0/docs/index.rst
--rw-r--r--   0        0        0     1427 2024-04-21 05:40:56.126496 oembedpy-0.5.0/docs/integrations/sphinx.rst
--rw-r--r--   0        0        0      800 2024-04-21 05:40:56.126496 oembedpy-0.5.0/docs/make.bat
--rw-r--r--   0        0        0       55 2024-04-21 05:40:56.126496 oembedpy-0.5.0/oembedpy/__init__.py
--rw-r--r--   0        0        0     1278 2024-04-21 05:40:56.126496 oembedpy-0.5.0/oembedpy/application.py
--rw-r--r--   0        0        0     1894 2024-04-21 05:40:56.126496 oembedpy-0.5.0/oembedpy/cli.py
--rw-r--r--   0        0        0     2067 2024-04-21 05:40:56.126496 oembedpy-0.5.0/oembedpy/consumer.py
--rw-r--r--   0        0        0     1995 2024-04-21 05:40:56.126496 oembedpy-0.5.0/oembedpy/discovery.py
--rw-r--r--   0        0        0       13 2024-04-21 05:40:56.126496 oembedpy-0.5.0/oembedpy/ext/__init__.py
--rw-r--r--   0        0        0     1695 2024-04-21 05:40:56.126496 oembedpy-0.5.0/oembedpy/ext/sphinx.py
--rw-r--r--   0        0        0     2693 2024-04-21 05:40:56.130496 oembedpy-0.5.0/oembedpy/provider.py
--rw-r--r--   0        0        0     2299 2024-04-21 05:40:56.130496 oembedpy-0.5.0/oembedpy/types.py
--rw-r--r--   0        0        0     1388 2024-04-21 05:40:56.130496 oembedpy-0.5.0/pyproject.toml
--rw-r--r--   0        0        0       83 2024-04-21 05:40:56.130496 oembedpy-0.5.0/tests/conftest.py
--rw-r--r--   0        0        0      145 2024-04-21 05:40:56.130496 oembedpy-0.5.0/tests/roots/test-default/conf.py
--rw-r--r--   0        0        0      378 2024-04-21 05:40:56.130496 oembedpy-0.5.0/tests/roots/test-default/index.rst
--rw-r--r--   0        0        0     4231 2024-04-21 05:40:56.130496 oembedpy-0.5.0/tests/test_consumer.py
--rw-r--r--   0        0        0     3649 2024-04-21 05:40:56.130496 oembedpy-0.5.0/tests/test_discovery.py
--rw-r--r--   0        0        0      979 2024-04-21 05:40:56.130496 oembedpy-0.5.0/tests/test_ext_sphinx.py
--rw-r--r--   0        0        0     1311 2024-04-21 05:40:56.130496 oembedpy-0.5.0/tests/test_provider.py
--rw-r--r--   0        0        0     2677 1970-01-01 00:00:00.000000 oembedpy-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0      861 2024-04-29 10:19:31.356193 oembedpy-0.6.0/.age.toml
+-rw-r--r--   0        0        0      560 2024-04-29 10:19:31.356193 oembedpy-0.6.0/.editorconfig
+-rw-r--r--   0        0        0      159 2024-04-29 10:19:31.356193 oembedpy-0.6.0/.github/release-body.md
+-rw-r--r--   0        0        0     1784 2024-04-29 10:19:31.356193 oembedpy-0.6.0/.github/workflows/main.yml
+-rwxr-xr-x   0        0        0     2695 2024-04-29 10:19:31.356193 oembedpy-0.6.0/.github/workflows/release.yml
+-rw-r--r--   0        0        0     3338 2024-04-29 10:19:31.356193 oembedpy-0.6.0/.gitignore
+-rw-r--r--   0        0        0      333 2024-04-29 10:19:31.356193 oembedpy-0.6.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      500 2024-04-29 10:19:31.356193 oembedpy-0.6.0/.readthedocs.yml
+-rw-r--r--   0        0        0     2122 2024-04-29 10:19:31.356193 oembedpy-0.6.0/CHANGES.rst
+-rw-r--r--   0        0        0     9161 2024-04-29 10:19:31.356193 oembedpy-0.6.0/LICENSE
+-rw-r--r--   0        0        0     1299 2024-04-29 10:19:31.356193 oembedpy-0.6.0/README.rst
+-rw-r--r--   0        0        0        5 2024-04-29 10:19:31.356193 oembedpy-0.6.0/docs/.gitignore
+-rw-r--r--   0        0        0      699 2024-04-29 10:19:31.356193 oembedpy-0.6.0/docs/Makefile
+-rw-r--r--   0        0        0       89 2024-04-29 10:19:31.356193 oembedpy-0.6.0/docs/api.rst
+-rw-r--r--   0        0        0      211 2024-04-29 10:19:31.356193 oembedpy-0.6.0/docs/changelogs.rst
+-rw-r--r--   0        0        0      461 2024-04-29 10:19:31.356193 oembedpy-0.6.0/docs/commandline.rst
+-rw-r--r--   0        0        0      363 2024-04-29 10:19:31.360193 oembedpy-0.6.0/docs/conf.py
+-rw-r--r--   0        0        0      390 2024-04-29 10:19:31.360193 oembedpy-0.6.0/docs/index.rst
+-rw-r--r--   0        0        0     1726 2024-04-29 10:19:31.360193 oembedpy-0.6.0/docs/integrations/sphinx.rst
+-rw-r--r--   0        0        0      800 2024-04-29 10:19:31.360193 oembedpy-0.6.0/docs/make.bat
+-rw-r--r--   0        0        0     1381 2024-04-29 10:19:31.360193 oembedpy-0.6.0/docs/workspace.rst
+-rw-r--r--   0        0        0       55 2024-04-29 10:19:31.360193 oembedpy-0.6.0/oembedpy/__init__.py
+-rw-r--r--   0        0        0     3228 2024-04-29 10:19:31.360193 oembedpy-0.6.0/oembedpy/application.py
+-rw-r--r--   0        0        0     2076 2024-04-29 10:19:31.360193 oembedpy-0.6.0/oembedpy/cli.py
+-rw-r--r--   0        0        0     2170 2024-04-29 10:19:31.360193 oembedpy-0.6.0/oembedpy/consumer.py
+-rw-r--r--   0        0        0     1821 2024-04-29 10:19:31.360193 oembedpy-0.6.0/oembedpy/discovery.py
+-rw-r--r--   0        0        0       13 2024-04-29 10:19:31.360193 oembedpy-0.6.0/oembedpy/ext/__init__.py
+-rw-r--r--   0        0        0     1969 2024-04-29 10:19:31.360193 oembedpy-0.6.0/oembedpy/ext/sphinx.py
+-rw-r--r--   0        0        0     2693 2024-04-29 10:19:31.360193 oembedpy-0.6.0/oembedpy/provider.py
+-rw-r--r--   0        0        0     2386 2024-04-29 10:19:31.360193 oembedpy-0.6.0/oembedpy/types.py
+-rw-r--r--   0        0        0     1473 2024-04-29 10:19:31.360193 oembedpy-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0       83 2024-04-29 10:19:31.360193 oembedpy-0.6.0/tests/conftest.py
+-rw-r--r--   0        0        0      145 2024-04-29 10:19:31.360193 oembedpy-0.6.0/tests/roots/test-default/conf.py
+-rw-r--r--   0        0        0      378 2024-04-29 10:19:31.360193 oembedpy-0.6.0/tests/roots/test-default/index.rst
+-rw-r--r--   0        0        0     2824 2024-04-29 10:19:31.360193 oembedpy-0.6.0/tests/test_application.py
+-rw-r--r--   0        0        0     4231 2024-04-29 10:19:31.360193 oembedpy-0.6.0/tests/test_consumer.py
+-rw-r--r--   0        0        0     3649 2024-04-29 10:19:31.360193 oembedpy-0.6.0/tests/test_discovery.py
+-rw-r--r--   0        0        0      979 2024-04-29 10:19:31.360193 oembedpy-0.6.0/tests/test_ext_sphinx.py
+-rw-r--r--   0        0        0     1311 2024-04-29 10:19:31.360193 oembedpy-0.6.0/tests/test_provider.py
+-rw-r--r--   0        0        0     2854 1970-01-01 00:00:00.000000 oembedpy-0.6.0/PKG-INFO
```

### Comparing `oembedpy-0.5.0/.age.toml` & `oembedpy-0.6.0/.age.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-current_version = "0.5.0"
+current_version = "0.6.0"
 
 [[files]]
 path = "oembedpy/__init__.py"
 search = "__version__ = \"{{current_version}}\""
 replace = "__version__ = \"{{new_version}}\""
 
 [[files]]
```

### Comparing `oembedpy-0.5.0/.editorconfig` & `oembedpy-0.6.0/.editorconfig`

 * *Files identical despite different names*

### Comparing `oembedpy-0.5.0/.github/workflows/main.yml` & `oembedpy-0.6.0/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `oembedpy-0.5.0/.github/workflows/release.yml` & `oembedpy-0.6.0/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `oembedpy-0.5.0/.gitignore` & `oembedpy-0.6.0/.gitignore`

 * *Files identical despite different names*

### Comparing `oembedpy-0.5.0/CHANGES.rst` & `oembedpy-0.6.0/CHANGES.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,26 @@
 ===========
 Change logs
 ===========
 
+v0.6.0
+======
+
+:date: 2024-04-29 (JST)
+
+Features
+--------
+
+* "workspace" to cache responses (optnional)
+
+Fixes
+-----
+
+* Reduce requests to providers.json
+
 v0.5.0
 ======
 
 :date: 2024-04-21 (JST)
 
 Features
 --------
```

### Comparing `oembedpy-0.5.0/LICENSE` & `oembedpy-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `oembedpy-0.5.0/README.rst` & `oembedpy-0.6.0/README.rst`

 * *Files identical despite different names*

### Comparing `oembedpy-0.5.0/docs/Makefile` & `oembedpy-0.6.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `oembedpy-0.5.0/docs/integrations/sphinx.rst` & `oembedpy-0.6.0/docs/integrations/sphinx.rst`

 * *Files 22% similar despite different names*

```diff
@@ -24,14 +24,29 @@
 
 .. code-block:: rst
 
    .. oembed:: CONTENT-URL
 
 When it build, embed ``iframe`` content into your HTML.
 
+Configuration
+-------------
+
+.. confval:: oembed_use_workspace
+
+   :Type: ``bool``
+   :Default: ``False``
+
+   Switch to toggle using simple client and workspace.
+
+   If it is set ``True```, extension uses ``Workspace`` object as client.
+
+   .. note:: See :doc:`../workspace` for more information.
+
+
 Spec of directive
 -----------------
 
 .. rst:directive:: oembed
 
    .. rst:directive:option:: maxwidth
       :type: int
```

### Comparing `oembedpy-0.5.0/docs/make.bat` & `oembedpy-0.6.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `oembedpy-0.5.0/oembedpy/cli.py` & `oembedpy-0.6.0/oembedpy/cli.py`

 * *Files 9% similar despite different names*

```diff
@@ -19,39 +19,44 @@
 
 
 @click.command
 @click.option(
     "--version", is_flag=True, default=False, help="Show version information and exit."
 )
 @click.option(
+    "-w", "--workspace", is_flag=True, default=False, help="Use caching workspace."
+)
+@click.option(
     "--format",
     type=click.Choice(["text", "json"]),
     default="text",
     help="Display JSON format.",
 )
 @click.option("--max-width", type=int, help="Max width for oEmbed content.")
 @click.option("--max-height", type=int, help="Max height for oEmbed content.")
 @click.argument("url")
 @click.pass_context
 def cli(
     ctx: click.Context,
     version: bool,
+    workspace: bool,
     url: str,
     format: OUTPUT_FORMAT,
     max_width: Optional[int] = None,
     max_height: Optional[int] = None,
 ):
     """Fetch and display oEmbed parameters from oEmbed provider."""
     if version:
         click.echo(f"{ctx.info_name} v{__version__}")
         ctx.exit(0)
 
     # Fetch content to find meta tags.
     logger.debug(f"Target Content URL is {url}")
-    oembed = application.Oembed()
+    oembed = application.Workspace() if workspace else application.Oembed()
+    oembed.init()
     try:
         content = oembed.fetch(url, max_width, max_height)
     except Exception as err:
         click.echo(click.style(f"Failed to oEmbed URL for {err}", fg="red"))
         ctx.abort()
 
     # Display data
```

### Comparing `oembedpy-0.5.0/oembedpy/consumer.py` & `oembedpy-0.6.0/oembedpy/consumer.py`

 * *Files 16% similar despite different names*

```diff
@@ -17,14 +17,17 @@
     """Supported query parameters."""
 
     url: str
     format: Optional[str] = None
     max_width: Optional[int] = None
     max_height: Optional[int] = None
 
+    def __hash__(self):
+        return hash((self.url, self.format, self.max_width, self.max_height))
+
     def to_dict(self) -> Dict[str, str]:
         """Make dict object from properties."""
         data = {"url": self.url}
         if self.max_width:
             data["maxwidth"] = str(self.max_width)
         if self.max_height:
             data["maxheight"] = str(self.max_height)
```

### Comparing `oembedpy-0.5.0/oembedpy/discovery.py` & `oembedpy-0.6.0/oembedpy/discovery.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Discovery module.
 
 This provides features to find oEmbed provider of contents.
 """
 
 import logging
 import urllib.parse
-from typing import Optional, Tuple
+from typing import Tuple
 
 import httpx
 from bs4 import BeautifulSoup
 
 from .consumer import RequestParameters
 from .provider import ProviderRegistry
 
@@ -46,21 +46,17 @@
         params.max_height = int(qs["maxheight"][0])
     if "format" in qs:
         params.format = qs["format"][0]
     return f"{parts.scheme}://{parts.netloc}{parts.path}", params
 
 
 def find_from_registry(
-    url: str, registry: Optional[ProviderRegistry] = None
+    url: str, registry: ProviderRegistry
 ) -> Tuple[str, RequestParameters]:
     """Find endpoint matched for content from registry."""
-    if registry is None:
-        resp = httpx.get("https://oembed.com/providers.json")
-        registry = ProviderRegistry.from_dict(resp.json())
-
     for provider in registry.providers:
         api_url = provider.find_endpoint(url)
         if api_url:
             return api_url, RequestParameters(url=url)
 
     msg = "Endpoint is not found from registry."
     logger.warning(msg)
```

### Comparing `oembedpy-0.5.0/oembedpy/ext/sphinx.py` & `oembedpy-0.6.0/oembedpy/ext/sphinx.py`

 * *Files 27% similar despite different names*

```diff
@@ -2,25 +2,26 @@
 
 import logging
 
 try:
     from docutils import nodes
     from docutils.parsers.rst import Directive, directives
     from sphinx.application import Sphinx
+    from sphinx.config import Config
 
     logger = logging.getLogger(__name__)
 except ModuleNotFoundError as err:
     logger = logging.getLogger(__name__)
 
     msg = "To use it, install with Sphinx."
     logging.error(msg)
     raise err
 
 from oembedpy import __version__
-from oembedpy.application import Oembed
+from oembedpy.application import Oembed, Workspace
 
 _oembed: Oembed
 
 
 class oembed(nodes.General, nodes.Element):  # noqa: D101,E501
     pass
 
@@ -51,20 +52,26 @@
         self.body.append(node["content"].html)
 
 
 def depart_oembed_node(self, node):  # noqa: D103
     pass
 
 
-def setup(app: Sphinx):  # noqa: D103
+def _init_client(app: Sphinx, config: Config):
     global _oembed
+    _oembed = Workspace() if config.oembed_use_workspace else Oembed()
+    _oembed.init()
+
+
+def setup(app: Sphinx):  # noqa: D103
+    app.add_config_value("oembed_use_workspace", False, "env")
     app.add_directive("oembed", OembedDirective)
     app.add_node(
         oembed,
         html=(visit_oembed_node, depart_oembed_node),
     )
-    _oembed = Oembed()
+    app.connect("config-inited", _init_client)
     return {
         "version": __version__,
         "parallel_read_safe": True,
         "parallel_write_safe": True,
     }
```

### Comparing `oembedpy-0.5.0/oembedpy/provider.py` & `oembedpy-0.6.0/oembedpy/provider.py`

 * *Files identical despite different names*

### Comparing `oembedpy-0.5.0/oembedpy/types.py` & `oembedpy-0.6.0/oembedpy/types.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 All typed classes are based from oEmbed specs.
 Please see https://oembed.com/
 """
 
 from dataclasses import asdict, dataclass
 from inspect import signature
-from typing import Any, Dict, Optional, Type, TypeVar, Union
+from typing import Any, Dict, NamedTuple, Optional, Type, TypeVar, Union
 
 T = TypeVar("T", bound="_Required")
 
 
 @dataclass
 class _Required:
     """Fields of required parameters for any types."""
@@ -99,7 +99,12 @@
 @dataclass
 class Rich(_Optionals, _Rich, _Required):
     """oEmbed content for rich HTML object."""
 
 
 Content = Union[Photo, Video, Link, Rich]
 """Collection of oEmbed content types."""
+
+
+class CachedContent(NamedTuple):
+    expired: float
+    content: Content
```

### Comparing `oembedpy-0.5.0/pyproject.toml` & `oembedpy-0.6.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -23,31 +23,35 @@
   "Topic :: Internet :: WWW/HTTP",
   "Topic :: Utilities",
 ]
 dependencies = [
   "beautifulsoup4",
   "httpx",
   "lxml",
+  "platformdirs",
 ]
 dynamic = ["version", "description"]
 
 [project.optional-dependencies]
 cli = ["Click>=8"]
 doc = [
   "furo",
   "Sphinx",
+  "sphinx-toolbox",
+  "rst-package-refs",
 ]
 sphinx = [
   "sphinx",
 ]
 test = [
   "sphinx[test]",
   "pytest==7.*",
   "pytest-cov==4.*",
   "pytest-httpx==0.21.*",
+  "pytest-mock==3.14.*",
 ]
 
 [project.scripts]
 "oEmbed.py" = "oembedpy.cli:main"
 
 [project.urls]
 Home = "https://github.com/attakei-lab/oEmbedPy"
```

### Comparing `oembedpy-0.5.0/tests/test_consumer.py` & `oembedpy-0.6.0/tests/test_consumer.py`

 * *Files identical despite different names*

### Comparing `oembedpy-0.5.0/tests/test_discovery.py` & `oembedpy-0.6.0/tests/test_discovery.py`

 * *Files identical despite different names*

### Comparing `oembedpy-0.5.0/tests/test_ext_sphinx.py` & `oembedpy-0.6.0/tests/test_ext_sphinx.py`

 * *Files identical despite different names*

### Comparing `oembedpy-0.5.0/tests/test_provider.py` & `oembedpy-0.6.0/tests/test_provider.py`

 * *Files identical despite different names*

### Comparing `oembedpy-0.5.0/PKG-INFO` & `oembedpy-0.6.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oEmbedPy
-Version: 0.5.0
+Version: 0.6.0
 Summary: oEmbed client for Python.
 Author-email: Kazuya Takei <myself@attakei.net>
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
@@ -17,22 +17,26 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Internet
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Utilities
 Requires-Dist: beautifulsoup4
 Requires-Dist: httpx
 Requires-Dist: lxml
+Requires-Dist: platformdirs
 Requires-Dist: Click>=8 ; extra == "cli"
 Requires-Dist: furo ; extra == "doc"
 Requires-Dist: Sphinx ; extra == "doc"
+Requires-Dist: sphinx-toolbox ; extra == "doc"
+Requires-Dist: rst-package-refs ; extra == "doc"
 Requires-Dist: sphinx ; extra == "sphinx"
 Requires-Dist: sphinx[test] ; extra == "test"
 Requires-Dist: pytest==7.* ; extra == "test"
 Requires-Dist: pytest-cov==4.* ; extra == "test"
 Requires-Dist: pytest-httpx==0.21.* ; extra == "test"
+Requires-Dist: pytest-mock==3.14.* ; extra == "test"
 Project-URL: Home, https://github.com/attakei-lab/oEmbedPy
 Provides-Extra: cli
 Provides-Extra: doc
 Provides-Extra: sphinx
 Provides-Extra: test
 
 ========
```

