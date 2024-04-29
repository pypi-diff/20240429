# Comparing `tmp/yaconfiglib-0.1.1.tar.gz` & `tmp/yaconfiglib-0.2.0.tar.gz`

## Comparing `yaconfiglib-0.1.1.tar` & `yaconfiglib-0.2.0.tar`

### file list

```diff
@@ -1,21 +1,23 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 yaconfiglib-0.1.1/examples/config.toml
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 yaconfiglib-0.1.1/examples/hiera.yaml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 yaconfiglib-0.1.1/examples/includeme.yaml
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 yaconfiglib-0.1.1/examples/jinja.yaml.j2
--rw-r--r--   0        0        0      880 2020-02-02 00:00:00.000000 yaconfiglib-0.1.1/src/example.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 yaconfiglib-0.1.1/src/yaconfiglib/__init__.py
--rw-r--r--   0        0        0     5942 2020-02-02 00:00:00.000000 yaconfiglib-0.1.1/src/yaconfiglib/hiera.py
--rw-r--r--   0        0        0     2213 2020-02-02 00:00:00.000000 yaconfiglib-0.1.1/src/yaconfiglib/jinja2.py
--rw-r--r--   0        0        0     6597 2020-02-02 00:00:00.000000 yaconfiglib-0.1.1/src/yaconfiglib/loader.py
--rw-r--r--   0        0        0     2510 2020-02-02 00:00:00.000000 yaconfiglib-0.1.1/src/yaconfiglib/reader.py
--rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 yaconfiglib-0.1.1/src/yaconfiglib/toml.py
--rw-r--r--   0        0        0     1550 2020-02-02 00:00:00.000000 yaconfiglib-0.1.1/src/yaconfiglib/yaml.py
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 yaconfiglib-0.1.1/src/yaconfiglib/utils/__init__.py
--rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 yaconfiglib-0.1.1/src/yaconfiglib/utils/enum.py
--rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 yaconfiglib-0.1.1/src/yaconfiglib/utils/log.py
--rw-r--r--   0        0        0    13130 2020-02-02 00:00:00.000000 yaconfiglib-0.1.1/src/yaconfiglib/utils/merge.py
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 yaconfiglib-0.1.1/.gitignore
--rw-r--r--   0        0        0    35823 2020-02-02 00:00:00.000000 yaconfiglib-0.1.1/LICENSE
--rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 yaconfiglib-0.1.1/README.md
--rw-r--r--   0        0        0      874 2020-02-02 00:00:00.000000 yaconfiglib-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1201 2020-02-02 00:00:00.000000 yaconfiglib-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 yaconfiglib-0.2.0/examples/config.toml
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 yaconfiglib-0.2.0/examples/hiera.yaml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 yaconfiglib-0.2.0/examples/includeme.yaml
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 yaconfiglib-0.2.0/examples/jinja.yaml.j2
+-rw-r--r--   0        0        0     1691 2020-02-02 00:00:00.000000 yaconfiglib-0.2.0/src/example.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 yaconfiglib-0.2.0/src/yaconfiglib/__init__.py
+-rw-r--r--   0        0        0     6307 2020-02-02 00:00:00.000000 yaconfiglib-0.2.0/src/yaconfiglib/hiera.py
+-rw-r--r--   0        0        0     7135 2020-02-02 00:00:00.000000 yaconfiglib-0.2.0/src/yaconfiglib/loader.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 yaconfiglib-0.2.0/src/yaconfiglib/backends/__init__.py
+-rw-r--r--   0        0        0     1640 2020-02-02 00:00:00.000000 yaconfiglib-0.2.0/src/yaconfiglib/backends/base.py
+-rw-r--r--   0        0        0     1333 2020-02-02 00:00:00.000000 yaconfiglib-0.2.0/src/yaconfiglib/backends/jinja2.py
+-rw-r--r--   0        0        0      435 2020-02-02 00:00:00.000000 yaconfiglib-0.2.0/src/yaconfiglib/backends/toml.py
+-rw-r--r--   0        0        0     2121 2020-02-02 00:00:00.000000 yaconfiglib-0.2.0/src/yaconfiglib/backends/yaml.py
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 yaconfiglib-0.2.0/src/yaconfiglib/utils/__init__.py
+-rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 yaconfiglib-0.2.0/src/yaconfiglib/utils/enum.py
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 yaconfiglib-0.2.0/src/yaconfiglib/utils/jinja2.py
+-rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 yaconfiglib-0.2.0/src/yaconfiglib/utils/log.py
+-rw-r--r--   0        0        0    16694 2020-02-02 00:00:00.000000 yaconfiglib-0.2.0/src/yaconfiglib/utils/merge.py
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 yaconfiglib-0.2.0/.gitignore
+-rw-r--r--   0        0        0    35823 2020-02-02 00:00:00.000000 yaconfiglib-0.2.0/LICENSE
+-rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 yaconfiglib-0.2.0/README.md
+-rw-r--r--   0        0        0      874 2020-02-02 00:00:00.000000 yaconfiglib-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1201 2020-02-02 00:00:00.000000 yaconfiglib-0.2.0/PKG-INFO
```

### Comparing `yaconfiglib-0.1.1/src/yaconfiglib/hiera.py` & `yaconfiglib-0.2.0/src/yaconfiglib/hiera.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,36 +1,38 @@
 import io
 import typing
 
 from pathlib_next import Path
+from pathlib_next.mempath import MemPath
 
-from yaconfiglib.jinja2 import jinja2_compile, jinja2_eval
+from yaconfiglib.utils import jinja2
 
 from . import loader
 from .utils import Logger, LogLevel, getLogger
 from .utils.merge import Merge, MergeMethod
 
 LOGGER = getLogger(LogLevel.Warning, __name__)
 
 
 def interpolate(data: object, globals: dict = None, logger: Logger = None):
     globals = {} if globals is None else globals
+    logger = logger or LOGGER
     logger.debug(
         'interpolate "%s" of type %s ...'
         % (
             data,
             type(data),
         )
     )
     if isinstance(data, str):
         _template = data.removeprefix("{{").removesuffix("}}")
         if not "{{" in _template and _template != data:
-            template = jinja2_eval(_template)
+            template = jinja2.eval(_template)
         else:
-            template = jinja2_compile(data)
+            template = jinja2.compile(data)
 
         _data = template(**globals)
         if not data == _data:
             logger.debug(
                 'interpolated "%s" to "%s" (type: %s)'
                 % (
                     data,
@@ -45,22 +47,25 @@
         keys = list(data.keys())
         for key in keys:
             value = data.pop(key)
             key = interpolate(key, globals, logger)
             data[key] = interpolate(value, globals, logger)
 
     elif isinstance(data, typing.Iterable):
-        if not isinstance(data, list):
+        if not isinstance(data, typing.MutableSequence):
             data = [*data]
         for idx, value in enumerate(data):
             data[idx] = interpolate(value, globals, logger)
 
     return data
 
 
+_interpolate = interpolate
+
+
 class HieraConfigLoader:
 
     DEFAULT_ENCODING: str = "utf-8"
 
     def __init__(
         self,
         merge: MergeMethod | Merge = MergeMethod.Simple,
@@ -75,87 +80,95 @@
         self.merge_options = {} if merge_options is None else merge_options
         self.interpolate = True if interpolate is None else bool(interpolate)
         self.backend = backend or loader.DEFAULT_LOADER
         self.missingfiles_level = LogLevel(missingfiles_level or LogLevel.Error)
         self.encoding = encoding or self.DEFAULT_ENCODING
         self.logger = getLogger(logger)
 
-    def load(self, *sources: str | Path):
+    def load(
+        self,
+        *sources: str | Path,
+        config_backend: loader.ConfigBackend = None,
+        interpolate: bool = None,
+        **backend_args,
+    ):
         data = None
-        for source in self._validate_sources(sources):
-            self.logger.debug("source: %s ..." % source)
-            if not source:
-                continue
-            if source.startswith("#!"):
-                filename, source = source.split("\n", maxsplit=1)
-                self.logger.debug("loading config doc from str ...")
-                filename = filename.removeprefix("#!")
-                f = io.StringIO(source)
-                data = self._load_data(f, data, filename=filename)
-            else:
-                path = Path(source) if not isinstance(source, Path) else source
+        backend = config_backend or self.backend
+        interpolate = self.interpolate if interpolate is None else interpolate
+        if interpolate:
+            interpolate = _interpolate
 
-                try:
-                    with path.open("r", encoding=self.encoding) as f:
-                        self.logger.debug("open4reading: file %s" % f)
-                        data = self._load_data(f, data, filename=path.name)
-                except IOError as e:
-                    if self.missingfiles_level >= LogLevel.Error:
-                        self.logger.log(self.missingfiles_level, e)
-                        self.logger.log(
-                            self.missingfiles_level,
-                            "file not found: %s" % source,
+        for source in self._validate_sources(sources):
+            try:
+                self.logger.debug("source: %s ..." % source)
+                for ydata in backend.load_all(source, **backend_args):
+                    if self.logger.isEnabledFor(LogLevel.Debug):
+                        self.logger.debug("config data: %s" % ydata)
+                    if data is None:
+                        data = ydata
+                    else:
+                        data = self.merge(
+                            data, ydata, logger=self.logger, **self.merge_options
                         )
-                        raise FileNotFoundError(source)
+                        self.logger.debug("merged data: %s" % data)
+            except IOError as e:
+                if self.missingfiles_level >= LogLevel.Error:
                     self.logger.log(self.missingfiles_level, e)
-                    continue
-        if self.interpolate:
-            data = interpolate(data, data, self.logger)
-
-        return data
+                    self.logger.log(
+                        self.missingfiles_level,
+                        "file not found: %s" % source,
+                    )
+                    raise FileNotFoundError(source)
+                self.logger.log(self.missingfiles_level, e)
+                continue
 
-    def _load_data(self, f: str | io.IOBase, data: object, **load_options):
-        for ydata in self.backend.load_all(f, **load_options):
-            if self.logger.isEnabledFor(LogLevel.Debug):
-                self.logger.debug("config data: %s" % ydata)
-            if data is None:
-                data = ydata
-            else:
-                data = self.merge(data, ydata, logger=self.logger, **self.merge_options)
-                self.logger.debug("merged data: %s" % data)
-        return data
+        return interpolate(data, data, self.logger) if interpolate else data
 
     def _validate_sources(
         self,
         sources: typing.Sequence[str | Path | typing.Sequence[str | Path]],
         *,
         memo: list[str | Path] = None,
-    ) -> typing.Iterator[str | Path]:
+    ) -> typing.Iterator[Path]:
         if memo is None:
             memo = []
         for source in sources:
+            if not source:
+                continue
             if isinstance(source, (str, Path)):
                 if source in memo:
                     self.logger.warning("ignoring duplicated file %s" % source)
                     continue
-                yield source
+                if source.startswith("#!"):
+                    filename, source = source.split("\n", maxsplit=1)
+                    self.logger.debug("loading config doc from str ...")
+                    filename = filename.removeprefix("#!")
+                    path = MemPath(filename)
+                    path.parent.mkdir(parents=True, exist_ok=True)
+                    path.write_text(source, encoding=self.encoding)
+                else:
+                    path = Path(source) if not isinstance(source, Path) else source
+                yield path
             elif isinstance(source, typing.Sequence):
                 yield from self._validate_sources(source, memo=memo)
             else:
                 raise ValueError(
                     "unable to handle arg %s of type %s"
                     % (
                         source,
                         type(source),
                     )
                 )
 
-    def dump(self, data: object, **kwds):
+    def dump(
+        self, data: object, *, config_backend: loader.ConfigBackend = None, **kwds
+    ):
         """dump the data as string"""
-        return self.backend.dumps(data, **kwds)
+        backend = config_backend or self.backend
+        return backend.dumps(data, **kwds)
 
 
 DEFAULT_LOADER = HieraConfigLoader()
 
 
 def dump(*args, **kwds):
     """dump the data as config"""
```

### Comparing `yaconfiglib-0.1.1/src/yaconfiglib/loader.py` & `yaconfiglib-0.2.0/src/yaconfiglib/loader.py`

 * *Files 21% similar despite different names*

```diff
@@ -2,57 +2,47 @@
 import logging
 import typing
 
 from pathlib_next import LocalPath, Path, Pathname, PosixPathname, glob
 from pathlib_next.mempath import MemPath
 
 try:
-    from .jinja2 import jinja2_eval
+    from .utils import jinja2
 except ImportError:
     ...
 
-from .reader import Reader
+from .backends.base import ConfigBackend
 
 _LOGGER = logging.getLogger("yaconfiglib")
 
 __all__ = ["Include"]
 
 
-class ConfigBackend(typing.Protocol):
-
-    def load(self, stream: io.IOBase, **options) -> object:
-        raise NotImplementedError()
-
-    def load_all(self, stream: io.IOBase, **options) -> typing.Iterable[object]:
-        yield self.load(stream, **options)
-
-    def dumps(self, data: str, **options) -> str:
-        raise NotImplementedError
-
-
 class ConfigLoader:
 
     DEFAULT_PATH_GENERATOR = LocalPath
     DEFAULT_ENCODING = "utf-8"
 
     def __init__(
         self,
         base_dir: str | Path = "",
         *,
         encoding: str = None,
         path_factory: typing.Callable[[str], Path] = None,
-        reader_factory: type[Reader] = None,
+        configloader_factory: type[ConfigBackend] = None,
         recursive: bool = None,
         key_factory: typing.Callable[[Path, object], str] = None,
     ) -> None:
         self.path_factory = path_factory or self.DEFAULT_PATH_GENERATOR
         self.base_dir = base_dir or ""
         self.encoding = encoding or self.DEFAULT_ENCODING
         self.recursive = False if recursive is None else recursive
-        self.reader_factory = reader_factory or Reader
+        self.configloader_factory = configloader_factory or (
+            lambda path: ConfigBackend.get_class_by_path(path)()
+        )
         self.key_factory = key_factory or (lambda path, value: path.stem)
 
     def _getpath(self, path: str | Path):
         return path if isinstance(path, Path) else self.path_factory(path)
 
     @property
     def base_dir(self):
@@ -60,52 +50,42 @@
 
     @base_dir.setter
     def base_dir(self, value: str | Path):
         self._base_dir = self._getpath(value)
 
     def _load(
         self,
-        pathname: Path | typing.Sequence[Path] | io.IOBase,
+        paths: typing.Iterable[Path],
         *,
+        encoding: str,
         recursive: bool = None,
-        encoding: str = None,
-        reader: str = None,
+        configloader: str = None,
         transform: str = None,
         key_factory: str | typing.Callable[[Path], str] = None,
         **reader_args,
-    ):
+    ) -> typing.Iterator[tuple[str, object]]:
 
-        encoding = encoding or self.encoding
         recursive = self.recursive if recursive is None else recursive
-        reader_factory = (
-            Reader.get_class_by_name(reader) if reader else self.reader_factory
-        )
-
-        if isinstance(pathname, io.IOBase):
-            text = pathname.read()
-            if isinstance(text, str):
-                text = text.encode()
-            filename = reader_args.get("filename", "unknown")
-            pathname = MemPath(filename)
-            pathname.write_bytes(text)
 
+        if isinstance(configloader, str):
+            configloader_factory = lambda path: ConfigBackend.get_class_by_name(
+                configloader
+            )(path)
+        elif callable(getattr(configloader, "load", None)):
+            configloader_factory = lambda path: configloader
         else:
-            pathname = (
-                [self.base_dir / path for path in pathname]
-                if not isinstance(pathname, (str, Pathname))
-                and isinstance(pathname, typing.Sequence)
-                else self.base_dir / pathname
-            )
+            configloader_factory = configloader or self.configloader_factory
+
+        if configloader is self:
+            configloader_factory = self.configloader_factory
 
-        paths = [pathname] if isinstance(pathname, Path) else pathname
-        results: list[tuple[str, object]] = []
         key_factory = key_factory or self.key_factory
         if not callable(key_factory):
             if key_factory.startswith("%"):
-                _eval = jinja2_eval(key_factory.removeprefix("%"))
+                _eval = jinja2.eval(key_factory.removeprefix("%"))
 
                 def _key(path: Path, value):
                     return _eval(value=value, pathname=PosixPathname(path.as_posix()))
 
             else:
                 _keyname = key_factory
 
@@ -115,58 +95,88 @@
                         val = val()
                     return str(val)
 
             key_factory = _key
         for _pathname in paths:
             for path in _pathname.glob("", recursive=self.recursive):
                 _LOGGER.debug(f"Loading file: {path}")
-                _reader = reader_factory(
-                    path,
-                    encoding=self.encoding,
+                _configloader = configloader_factory(path)
+                _options = dict(
+                    encoding=encoding,
                     path_factory=self.path_factory,
-                    reader_factory=self.reader_factory,
+                    configloader=self,
                     base_dir=self.base_dir,
-                    **reader_args,
                 )
-                value = _reader()
+                _options.update(reader_args)
+
+                value = _configloader.load(path, **_options)
                 if transform:
-                    value = jinja2_eval(transform)(
+                    value = jinja2.eval(transform)(
                         value=value, pathname=PosixPathname(path.as_posix())
                     )
 
-                results.append((key_factory(path, value), value))
-
-        return (
-            results,
-            isinstance(pathname, Pathname)
-            and glob.WILCARD_PATTERN.match(pathname.as_posix()) is None,
-        )
+                yield key_factory(path, value), value
 
     def load(
         self,
         pathname: Path | typing.Sequence[Path],
         *,
         recursive: bool = None,
         encoding: str = None,
-        reader: str = None,
+        configloader: str = None,
         transform: str = None,
         default: object = None,
         type: str = None,
         key_factory: str | typing.Callable[[Path], str] = None,
         flatten: bool = False,
         **reader_args,
     ):
-        results, single = self._load(
-            pathname,
-            recursive=recursive,
-            encoding=encoding,
-            reader=reader,
-            transform=transform,
-            key_factory=key_factory,
-            **reader_args,
+        encoding = encoding or self.encoding
+        paths: list[Path] = []
+        is_list = not isinstance(pathname, (str, Pathname)) and isinstance(
+            pathname, typing.Iterable
+        )
+        for path in pathname if is_list else [pathname]:
+            if isinstance(path, io.IOBase):
+                filename = reader_args.get("filename", "unknown")
+                content = path.read()
+                path = MemPath(filename)
+                path.parent.mkdir(parents=True, exist_ok=True)
+                if isinstance(content, str):
+                    path.write_text(content, encoding=encoding)
+                else:
+                    path.write_bytes(content)
+            elif isinstance(path, Path):
+                try:
+                    path = self.base_dir / path
+                except Exception as _e:
+                    ...
+            else:
+                path = self.base_dir / path
+            paths.append(path)
+
+        single = (
+            not is_list
+            or pathname
+            and glob.WILCARD_PATTERN.match(paths[0].as_posix()) is None
+        )
+        if not is_list:
+            pathname = paths[0]
+        else:
+            pathname = paths
+        results = list(
+            self._load(
+                paths,
+                recursive=recursive,
+                encoding=encoding,
+                configloader=configloader,
+                transform=transform,
+                key_factory=key_factory,
+                **reader_args,
+            )
         )
         if not type:
             type = "single" if single else "list"
         type = type.lower()
         match type:
             case "single" | "scalar":
                 return results[-1][1] if results else default
```

### Comparing `yaconfiglib-0.1.1/src/yaconfiglib/yaml.py` & `yaconfiglib-0.2.0/src/yaconfiglib/backends/yaml.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 import re
 import typing
 
 import yaml
 from pathlib_next import Path, Pathname
 
-from .loader import ConfigLoader
-from .reader import Reader
+from yaconfiglib.backends.base import ConfigBackend
 
-__all__ = ["YamlConfigLoader", "YamlReader"]
+__all__ = ["YamlConfigLoader"]
 
 
-class YamlConfigLoader(ConfigLoader):
+class YamlConfigLoader(ConfigBackend):
+    PATHNAME_REGEX = re.compile(r".*\.((yaml)|(yml))$", re.IGNORECASE)
+    DEFAULT_LOADER_CLS = yaml.SafeLoader
+    PATH_FACTORY = Path
+
     def __call__(self, loader: yaml.Loader, node: yaml.Node):
         args = ()
         kwargs = {}
         pathname: str | Pathname | typing.Sequence[str | Pathname]
         if isinstance(node, yaml.nodes.ScalarNode):
             pathname = loader.construct_scalar(node)
         elif isinstance(node, yaml.nodes.SequenceNode):
@@ -23,25 +26,38 @@
             kwargs = loader.construct_mapping(node, deep=True)
             pathname = kwargs.pop("pathname")
         else:
             raise TypeError(f"Un-supported YAML node {node!r}")
 
         return self.load(pathname, *args, **kwargs, loader=loader)
 
+    def load(
+        self,
+        path: Path | str,
+        encoding: str = None,
+        master: yaml.Loader = None,
+        loader_cls: type[yaml.Loader] = None,
+        path_factory: type[Path] = None,
+        configloader: type[ConfigBackend] = None,
+        **options,
+    ) -> object:
+
+        if path_factory is None:
+            path_factory = self.PATH_FACTORY
+        if isinstance(path, str):
+            path = path_factory(path)
+        if master and not loader_cls:
+            loader_cls = type(master)
+        if loader_cls is None:
+            loader_cls = self.DEFAULT_LOADER_CLS
 
-class YamlReader(Reader):
-    PATHNAME_REGEX = re.compile(r".*\.((yaml)|(yml))$", re.IGNORECASE)
-
-    def __init__(
-        self, path: Path, encoding: str, loader: yaml.Loader = None, **kwargs
-    ) -> None:
-        self.master = loader or yaml.SafeLoader("")
-        super().__init__(path, encoding, **kwargs)
+        if configloader and not self.can_load_path(path):
+            return configloader.load(path, loader_cls=loader_cls, encoding=encoding)
 
-    def __call__(self):
-        loader = type(self.master)(self.read_text())
+        loader = loader_cls(path.read_text(encoding=encoding))
         try:
-            loader.anchors = self.master.anchors
+            if master:
+                loader.anchors = master.anchors
             data = loader.get_single_data()
             return data
         finally:
             loader.dispose()
```

### Comparing `yaconfiglib-0.1.1/src/yaconfiglib/utils/log.py` & `yaconfiglib-0.2.0/src/yaconfiglib/utils/log.py`

 * *Files identical despite different names*

### Comparing `yaconfiglib-0.1.1/LICENSE` & `yaconfiglib-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `yaconfiglib-0.1.1/pyproject.toml` & `yaconfiglib-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "yaconfiglib"
-version = "0.1.1"
+version = "0.2.0"
 authors = [{ name = "Jose A" }]
 description = "Another Config lib for python, basically load config/yaml/toml/... files and add some features like relative import and templating."
 readme = "README.md"
 requires-python = ">=3.11"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
```

### Comparing `yaconfiglib-0.1.1/PKG-INFO` & `yaconfiglib-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: yaconfiglib
-Version: 0.1.1
+Version: 0.2.0
 Summary: Another Config lib for python, basically load config/yaml/toml/... files and add some features like relative import and templating.
 Project-URL: Homepage, https://github.com/jose-pr/yaconfiglib/
 Project-URL: Issues, https://github.com/jose-pr/yaconfiglib/issues
 Author: Jose A
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

