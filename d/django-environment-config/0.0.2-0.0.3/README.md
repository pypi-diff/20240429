# Comparing `tmp/django_environment_config-0.0.2.tar.gz` & `tmp/django_environment_config-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_environment_config-0.0.2.tar", max compression
+gzip compressed data, was "django_environment_config-0.0.3.tar", max compression
```

## Comparing `django_environment_config-0.0.2.tar` & `django_environment_config-0.0.3.tar`

### file list

```diff
@@ -1,11 +1,13 @@
--rw-r--r--   0        0        0     2705 2024-04-29 09:02:34.023885 django_environment_config-0.0.2/LICENSE
--rw-r--r--   0        0        0     2148 2024-04-29 09:02:34.023885 django_environment_config-0.0.2/README.md
--rw-r--r--   0        0        0       64 2024-04-29 09:02:34.023885 django_environment_config-0.0.2/env_config/__init__.py
--rw-r--r--   0        0        0     3006 2024-04-29 09:02:34.023885 django_environment_config-0.0.2/env_config/base.py
--rw-r--r--   0        0        0      306 2024-04-29 09:02:34.023885 django_environment_config-0.0.2/env_config/constants.py
--rw-r--r--   0        0        0      901 2024-04-29 09:02:34.023885 django_environment_config-0.0.2/env_config/errors.py
--rw-r--r--   0        0        0        0 2024-04-29 09:02:34.023885 django_environment_config-0.0.2/env_config/py.typed
--rw-r--r--   0        0        0     1210 2024-04-29 09:02:34.023885 django_environment_config-0.0.2/env_config/typing.py
--rw-r--r--   0        0        0    11566 2024-04-29 09:02:34.023885 django_environment_config-0.0.2/env_config/values.py
--rw-r--r--   0        0        0     8589 2024-04-29 09:02:34.023885 django_environment_config-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     3640 1970-01-01 00:00:00.000000 django_environment_config-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     2705 2024-04-29 11:00:57.074359 django_environment_config-0.0.3/LICENSE
+-rw-r--r--   0        0        0     2148 2024-04-29 11:00:57.074359 django_environment_config-0.0.3/README.md
+-rw-r--r--   0        0        0       64 2024-04-29 11:00:57.074359 django_environment_config-0.0.3/env_config/__init__.py
+-rw-r--r--   0        0        0     3206 2024-04-29 11:00:57.074359 django_environment_config-0.0.3/env_config/base.py
+-rw-r--r--   0        0        0      364 2024-04-29 11:00:57.074359 django_environment_config-0.0.3/env_config/constants.py
+-rw-r--r--   0        0        0      901 2024-04-29 11:00:57.074359 django_environment_config-0.0.3/env_config/errors.py
+-rw-r--r--   0        0        0        0 2024-04-29 11:00:57.074359 django_environment_config-0.0.3/env_config/py.typed
+-rw-r--r--   0        0        0     1210 2024-04-29 11:00:57.074359 django_environment_config-0.0.3/env_config/typing.py
+-rw-r--r--   0        0        0    11566 2024-04-29 11:00:57.074359 django_environment_config-0.0.3/env_config/values.py
+-rw-r--r--   0        0        0     8706 2024-04-29 11:00:57.074359 django_environment_config-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-29 11:00:57.074359 django_environment_config-0.0.3/pytest_plugin/__init__.py
+-rw-r--r--   0        0        0      792 2024-04-29 11:00:57.074359 django_environment_config-0.0.3/pytest_plugin/hooks.py
+-rw-r--r--   0        0        0     3640 1970-01-01 00:00:00.000000 django_environment_config-0.0.3/PKG-INFO
```

### Comparing `django_environment_config-0.0.2/LICENSE` & `django_environment_config-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `django_environment_config-0.0.2/README.md` & `django_environment_config-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `django_environment_config-0.0.2/env_config/base.py` & `django_environment_config-0.0.3/env_config/base.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import inspect
 import os
 from typing import TYPE_CHECKING
 
 from django.utils.functional import classproperty
 from dotenv import dotenv_values
 
-from .constants import Undefined
+from .constants import ENV_NAME, Undefined
 
 if TYPE_CHECKING:
     from dotenv.main import StrPath
 
     from .typing import Any
 
 __all__ = [
@@ -23,17 +23,17 @@
     """Configures a single environment."""
 
     def __init_subclass__(
         cls,
         *,
         dotenv_path: StrPath | None | Undefined = Undefined,
     ) -> None:
-        env: str | None = os.environ.get("DJANGO_SETTINGS_ENVIRONMENT")
+        env: str | None = os.environ.get(ENV_NAME)
         if env is None:  # pragma: no cover
-            msg = f"Environment variable 'DJANGO_SETTINGS_ENVIRONMENT' is not set before subclassing {cls.__name__!r}"
+            msg = f"Environment variable {ENV_NAME!r} must be set before subclassing {cls.__name__!r}"
             raise ValueError(msg)
 
         if cls.__name__ != env:
             return
 
         # If not given, set it to `None` so that `python-dotenv` will use
         # `dotenv.main.find_dotenv` to find the `.env` file automatically.
@@ -47,23 +47,31 @@
 
         # Do name mangling to avoid overriding the attribute from a parent class.
         # This way, we can have multiple environments with different `.env` files,
         # and allow using values from a parent `.env` file as defaults (if desired).
         setattr(cls, f"_{cls.__name__}__dotenv", dotenv)
         setattr(cls, f"_{cls.__name__}__dotenv_path", dotenv_path)
 
+        cls.pre_setup()
         cls.setup(stack_level=2)
         cls.post_setup()
 
     @staticmethod
     def load_dotenv(*, dotenv_path: StrPath | None = None) -> dict[str, str]:
         """Load the `.env` file and return the values."""
         return dotenv_values(dotenv_path=dotenv_path)
 
     @classmethod
+    def pre_setup(cls) -> None:
+        """
+        Hook for doing additional setup before the settings have been loaded,
+        but after the `.env` file has been loaded.
+        """
+
+    @classmethod
     def setup(cls, *, stack_level: int = 1) -> None:
         """Load settings and set them in the module globals where the environment is defined."""
         settings = cls.load_settings()
         stack = inspect.stack()
         caller_globals: dict[str, Any] = stack[stack_level].frame.f_globals
         caller_globals.update(**settings)
```

### Comparing `django_environment_config-0.0.2/env_config/errors.py` & `django_environment_config-0.0.3/env_config/errors.py`

 * *Files identical despite different names*

### Comparing `django_environment_config-0.0.2/env_config/typing.py` & `django_environment_config-0.0.3/env_config/typing.py`

 * *Files identical despite different names*

### Comparing `django_environment_config-0.0.2/env_config/values.py` & `django_environment_config-0.0.3/env_config/values.py`

 * *Files identical despite different names*

### Comparing `django_environment_config-0.0.2/pyproject.toml` & `django_environment_config-0.0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 [tool.poetry]
 name = "django-environment-config"
-version = "0.0.2"
+version = "0.0.3"
 description = "Configure django settings for multiple environments."
 authors = [
     "Matti Lamppu <lamppu.matti.akseli@gmail.com>",
 ]
 packages = [
     { include = "env_config" },
+    { include = "pytest_plugin" },
 ]
 license = "MIT"
 readme = "README.md"
 homepage = "https://mrthearman.github.io/django-environment-config"
 repository = "https://github.com/MrThearMan/django-environment-config"
 keywords = [
     "django",
@@ -70,14 +71,17 @@
 mypy = "1.10.0"
 django-stubs = "4.2.7"
 
 [tool.poetry.extras]
 db = ["dj-database-url"]
 cache = ["django-cache-url"]
 
+[tool.poetry.plugins.pytest11]
+django_environment_config = "pytest_plugin.hooks"
+
 [tool.ruff]
 fix = true
 unsafe-fixes = true
 line-length = 120
 extend-exclude = [
     "tests/*",
 ]
```

### Comparing `django_environment_config-0.0.2/PKG-INFO` & `django_environment_config-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-environment-config
-Version: 0.0.2
+Version: 0.0.3
 Summary: Configure django settings for multiple environments.
 Home-page: https://mrthearman.github.io/django-environment-config
 License: MIT
 Keywords: django,configuration,settings,environment,env,config
 Author: Matti Lamppu
 Author-email: lamppu.matti.akseli@gmail.com
 Requires-Python: >=3.10,<4
```

