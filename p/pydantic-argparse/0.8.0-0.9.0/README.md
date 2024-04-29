# Comparing `tmp/pydantic_argparse-0.8.0.tar.gz` & `tmp/pydantic_argparse-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydantic_argparse-0.8.0.tar", max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `pydantic_argparse-0.8.0.tar` & `pydantic_argparse-0.9.0.tar`

### file list

```diff
@@ -1,25 +1,28 @@
--rw-r--r--   0        0        0     1071 2022-10-08 08:09:10.000000 pydantic_argparse-0.8.0/LICENSE.md
--rw-r--r--   0        0        0     3681 2023-02-20 09:14:35.747805 pydantic_argparse-0.8.0/README.md
--rw-r--r--   0        0        0      866 2023-02-20 09:14:35.749133 pydantic_argparse-0.8.0/pydantic_argparse/__init__.py
--rw-r--r--   0        0        0      947 2023-02-20 09:14:35.749235 pydantic_argparse-0.8.0/pydantic_argparse/__metadata__.py
--rw-r--r--   0        0        0      520 2023-02-20 09:14:35.749344 pydantic_argparse-0.8.0/pydantic_argparse/argparse/__init__.py
--rw-r--r--   0        0        0     8973 2023-03-12 05:17:42.236678 pydantic_argparse-0.8.0/pydantic_argparse/argparse/actions.py
--rw-r--r--   0        0        0    11141 2023-03-12 05:17:42.236914 pydantic_argparse-0.8.0/pydantic_argparse/argparse/parser.py
--rw-r--r--   0        0        0     1849 2023-03-05 05:27:15.016054 pydantic_argparse-0.8.0/pydantic_argparse/argparse/patches.py
--rw-r--r--   0        0        0      657 2023-02-20 09:14:35.749812 pydantic_argparse-0.8.0/pydantic_argparse/parsers/__init__.py
--rw-r--r--   0        0        0     1969 2023-03-12 05:17:42.237122 pydantic_argparse-0.8.0/pydantic_argparse/parsers/boolean.py
--rw-r--r--   0        0        0     1554 2023-03-12 05:17:42.237315 pydantic_argparse-0.8.0/pydantic_argparse/parsers/command.py
--rw-r--r--   0        0        0     1869 2023-03-12 05:17:42.237510 pydantic_argparse-0.8.0/pydantic_argparse/parsers/container.py
--rw-r--r--   0        0        0     2279 2023-03-12 05:17:42.237737 pydantic_argparse-0.8.0/pydantic_argparse/parsers/enum.py
--rw-r--r--   0        0        0     2633 2023-03-12 05:17:42.238004 pydantic_argparse-0.8.0/pydantic_argparse/parsers/literal.py
--rw-r--r--   0        0        0     1722 2023-03-12 05:17:42.238228 pydantic_argparse-0.8.0/pydantic_argparse/parsers/mapping.py
--rw-r--r--   0        0        0     1426 2023-03-12 05:17:42.238430 pydantic_argparse-0.8.0/pydantic_argparse/parsers/standard.py
--rw-r--r--   0        0        0        0 2022-10-08 08:09:10.000000 pydantic_argparse-0.8.0/pydantic_argparse/py.typed
--rw-r--r--   0        0        0      725 2023-03-12 05:17:42.238659 pydantic_argparse-0.8.0/pydantic_argparse/utils/__init__.py
--rw-r--r--   0        0        0     1236 2023-03-12 05:17:42.238793 pydantic_argparse-0.8.0/pydantic_argparse/utils/arguments.py
--rw-r--r--   0        0        0      687 2023-03-12 05:17:42.238926 pydantic_argparse-0.8.0/pydantic_argparse/utils/errors.py
--rw-r--r--   0        0        0      916 2023-03-12 05:17:42.239062 pydantic_argparse-0.8.0/pydantic_argparse/utils/namespaces.py
--rw-r--r--   0        0        0     5280 2023-03-12 05:17:42.239201 pydantic_argparse-0.8.0/pydantic_argparse/utils/pydantic.py
--rw-r--r--   0        0        0     1872 2023-03-12 05:17:42.239398 pydantic_argparse-0.8.0/pydantic_argparse/utils/types.py
--rw-r--r--   0        0        0     2692 2023-03-12 06:00:48.783558 pydantic_argparse-0.8.0/pyproject.toml
--rw-r--r--   0        0        0     4622 1970-01-01 00:00:00.000000 pydantic_argparse-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 pydantic_argparse-0.9.0/src/pydantic_argparse/__init__.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 pydantic_argparse-0.9.0/src/pydantic_argparse/__metadata__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pydantic_argparse-0.9.0/src/pydantic_argparse/py.typed
+-rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 pydantic_argparse-0.9.0/src/pydantic_argparse/argparse/__init__.py
+-rw-r--r--   0        0        0     8999 2020-02-02 00:00:00.000000 pydantic_argparse-0.9.0/src/pydantic_argparse/argparse/actions.py
+-rw-r--r--   0        0        0    11139 2020-02-02 00:00:00.000000 pydantic_argparse-0.9.0/src/pydantic_argparse/argparse/parser.py
+-rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 pydantic_argparse-0.9.0/src/pydantic_argparse/compatibility/__init__.py
+-rw-r--r--   0        0        0     1837 2020-02-02 00:00:00.000000 pydantic_argparse-0.9.0/src/pydantic_argparse/compatibility/argparse.py
+-rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 pydantic_argparse-0.9.0/src/pydantic_argparse/compatibility/pydantic.py
+-rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 pydantic_argparse-0.9.0/src/pydantic_argparse/parsers/__init__.py
+-rw-r--r--   0        0        0     2016 2020-02-02 00:00:00.000000 pydantic_argparse-0.9.0/src/pydantic_argparse/parsers/boolean.py
+-rw-r--r--   0        0        0     1601 2020-02-02 00:00:00.000000 pydantic_argparse-0.9.0/src/pydantic_argparse/parsers/command.py
+-rw-r--r--   0        0        0     1928 2020-02-02 00:00:00.000000 pydantic_argparse-0.9.0/src/pydantic_argparse/parsers/container.py
+-rw-r--r--   0        0        0     2368 2020-02-02 00:00:00.000000 pydantic_argparse-0.9.0/src/pydantic_argparse/parsers/enum.py
+-rw-r--r--   0        0        0     2495 2020-02-02 00:00:00.000000 pydantic_argparse-0.9.0/src/pydantic_argparse/parsers/literal.py
+-rw-r--r--   0        0        0     1781 2020-02-02 00:00:00.000000 pydantic_argparse-0.9.0/src/pydantic_argparse/parsers/mapping.py
+-rw-r--r--   0        0        0     1473 2020-02-02 00:00:00.000000 pydantic_argparse-0.9.0/src/pydantic_argparse/parsers/standard.py
+-rw-r--r--   0        0        0      783 2020-02-02 00:00:00.000000 pydantic_argparse-0.9.0/src/pydantic_argparse/utils/__init__.py
+-rw-r--r--   0        0        0     1267 2020-02-02 00:00:00.000000 pydantic_argparse-0.9.0/src/pydantic_argparse/utils/arguments.py
+-rw-r--r--   0        0        0      718 2020-02-02 00:00:00.000000 pydantic_argparse-0.9.0/src/pydantic_argparse/utils/errors.py
+-rw-r--r--   0        0        0      950 2020-02-02 00:00:00.000000 pydantic_argparse-0.9.0/src/pydantic_argparse/utils/namespaces.py
+-rw-r--r--   0        0        0     5313 2020-02-02 00:00:00.000000 pydantic_argparse-0.9.0/src/pydantic_argparse/utils/pydantic.py
+-rw-r--r--   0        0        0     1713 2020-02-02 00:00:00.000000 pydantic_argparse-0.9.0/src/pydantic_argparse/utils/types.py
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 pydantic_argparse-0.9.0/.gitignore
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 pydantic_argparse-0.9.0/LICENSE
+-rw-r--r--   0        0        0     3779 2020-02-02 00:00:00.000000 pydantic_argparse-0.9.0/README.md
+-rw-r--r--   0        0        0     3060 2020-02-02 00:00:00.000000 pydantic_argparse-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0     6298 2020-02-02 00:00:00.000000 pydantic_argparse-0.9.0/PKG-INFO
```

### Comparing `pydantic_argparse-0.8.0/LICENSE.md` & `pydantic_argparse-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pydantic_argparse-0.8.0/README.md` & `pydantic_argparse-0.9.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -34,23 +34,26 @@
         <img src="https://img.shields.io/github/actions/workflow/status/supimdos/pydantic-argparse/typing.yml?label=typing">
     </a>
 </div>
 
 ## Help
 See [documentation](https://pydantic-argparse.supimdos.com) for help.
 
+## Requirements
+Requires Python 3.8+, and is compatible with the Pydantic v1 API.
+
 ## Installation
 Installation with `pip` is simple:
 ```console
 $ pip install pydantic-argparse
 ```
 
 ## Example
 ```py
-import pydantic
+import pydantic.v1 as pydantic
 import pydantic_argparse
 
 
 class Arguments(pydantic.BaseModel):
     # Required Args
     string: str = pydantic.Field(description="a required string")
     integer: int = pydantic.Field(description="a required integer")
```

### Comparing `pydantic_argparse-0.8.0/pydantic_argparse/__init__.py` & `pydantic_argparse-0.9.0/src/pydantic_argparse/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -5,24 +5,12 @@
 `pydantic` models.
 
 The public interface exposed by this package is the declarative and typed
 `ArgumentParser` class, as well as the package "dunder" metadata.
 """
 
 # Local
-from pydantic_argparse.argparse import ArgumentParser
-from pydantic_argparse.__metadata__ import __title__
-from pydantic_argparse.__metadata__ import __description__
-from pydantic_argparse.__metadata__ import __version__
-from pydantic_argparse.__metadata__ import __author__
-from pydantic_argparse.__metadata__ import __license__
-
-
-# Public Re-Exports
-__all__ = (
-    "ArgumentParser",
-    "__title__",
-    "__description__",
-    "__version__",
-    "__author__",
-    "__license__",
-)
+from pydantic_argparse.argparse import ArgumentParser as ArgumentParser
+from pydantic_argparse.__metadata__ import __version__ as __version__
+from pydantic_argparse.__metadata__ import __version_tuple__ as __version_tuple__
+from pydantic_argparse.__metadata__ import version as version
+from pydantic_argparse.__metadata__ import version_tuple as version_tuple
```

### Comparing `pydantic_argparse-0.8.0/pydantic_argparse/argparse/actions.py` & `pydantic_argparse-0.9.0/src/pydantic_argparse/argparse/actions.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 The `actions` module contains the `SubParsersAction` class, which is an action
 that provides recursive namespace nesting when parsing sub-commands. It also
 contains the `BooleanOptionalAction` class, which is a direct backport of the
 Python standard library `argparse` class of the same name.
 """
 
 
-# Standard
-import argparse
+# Local
+from pydantic_argparse.compatibility import argparse
 
 # Typing
 from typing import Any, Callable, Iterable, List, Optional, Sequence, Tuple, TypeVar, Union, cast
 
 
 # Constants
 T = TypeVar("T")
@@ -126,16 +126,16 @@
 
     This backported action provides the functionality for parsing paired
     GNU-style boolean arguments, such as "--foo/--no-foo". This style of
     argument allows us to easily provide *required* boolean arguments.
 
     This action was added into the Python standard library `argparse` module
     in [`BPO-8538`](https://bugs.python.org/issue8538) and is available in
-    Python 3.9 and above. In order to support Python 3.7 and 3.8 we directly
-    backport the class and make it available here.
+    Python 3.9 and above. In order to support Python 3.8 we directly backport
+    the class and make it available here.
 
     Source:
     <https://github.com/python/cpython/blob/v3.11.0/Lib/argparse.py#L878-L914>
     """
     def __init__(
         self,
         option_strings: Sequence[str],
```

### Comparing `pydantic_argparse-0.8.0/pydantic_argparse/argparse/parser.py` & `pydantic_argparse-0.9.0/src/pydantic_argparse/argparse/parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,25 +12,22 @@
 The resultant arguments object returned is an instance of the defined
 `pydantic` model. This means that the arguments object and its attributes will
 be compatible with an IDE, linter or type checker.
 """
 
 
 # Standard
-import argparse
 import sys
 
-# Third-Party
-import pydantic
-
 # Local
 from pydantic_argparse import parsers
 from pydantic_argparse import utils
 from pydantic_argparse.argparse import actions
-from pydantic_argparse.argparse import patches  # noqa: F401
+from pydantic_argparse.compatibility import argparse
+from pydantic_argparse.compatibility import pydantic
 
 # Typing
 from typing import Any, Dict, Generic, List, NoReturn, Optional, Type, TypeVar
 
 
 # Constants
 PydanticModelT = TypeVar("PydanticModelT", bound=pydantic.BaseModel)
```

### Comparing `pydantic_argparse-0.8.0/pydantic_argparse/argparse/patches.py` & `pydantic_argparse-0.9.0/src/pydantic_argparse/compatibility/argparse.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,26 @@
-"""Monkey patches for ArgumentParser.
+"""Compatibility Shim for ArgumentParser.
 
-In order to support Python 3.7 and 3.8 while retaining the unit tests, we need
-to backport the bugfix for [`BPO-29298`](https://bugs.python.org/issue29298).
+In order to support Python 3.8 while retaining the unit tests, we need to
+backport the bugfix for [`BPO-29298`](https://bugs.python.org/issue29298).
 """
 
 
 # Standard
 import argparse
 import sys
 
 # Typing
 from typing import Optional
 
 
 # In Python versions before 3.9, using argparse with required subparsers will
 # cause an unhelpful `TypeError` if the 'dest' parameter is not explicitly
 # specified, and no arguments are provided. This bug was fixed in 3.11 and
-# backported to 3.10 and 3.9. Here, we backport it to 3.7 and 3.8 as well, via
+# backported to 3.10 and 3.9. Here, we backport it to 3.8 as well, via
 # monkey-patching.
 # See: https://github.com/python/cpython/blob/v3.11.1/Lib/argparse.py#L739-L751
 if sys.version_info < (3, 9):  # pragma: <3.9 cover
     def _get_action_name(argument: Optional[argparse.Action]) -> Optional[str]:  # pragma: no cover
         """Generates the name for an argument action.
 
         The behaviour differs depending on what the action contains:
```

### Comparing `pydantic_argparse-0.8.0/pydantic_argparse/parsers/__init__.py` & `pydantic_argparse-0.9.0/src/pydantic_argparse/parsers/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -4,14 +4,14 @@
 fields to `ArgumentParser` command-line arguments.
 
 The public interface exposed by this package is the `parsing` modules, which
 each contain the `should_parse()` and `parse_field()` functions.
 """
 
 # Local
-from pydantic_argparse.parsers import boolean
-from pydantic_argparse.parsers import command
-from pydantic_argparse.parsers import container
-from pydantic_argparse.parsers import enum
-from pydantic_argparse.parsers import literal
-from pydantic_argparse.parsers import mapping
-from pydantic_argparse.parsers import standard
+from pydantic_argparse.parsers import boolean as boolean
+from pydantic_argparse.parsers import command as command
+from pydantic_argparse.parsers import container as container
+from pydantic_argparse.parsers import enum as enum
+from pydantic_argparse.parsers import literal as literal
+from pydantic_argparse.parsers import mapping as mapping
+from pydantic_argparse.parsers import standard as standard
```

### Comparing `pydantic_argparse-0.8.0/pydantic_argparse/parsers/boolean.py` & `pydantic_argparse-0.9.0/src/pydantic_argparse/parsers/boolean.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,26 +3,22 @@
 The `boolean` module contains the `should_parse` function, which checks whether
 this module should be used to parse the field, as well as the `parse_field`
 function, which parses boolean `pydantic` model fields to `ArgumentParser`
 command-line arguments.
 """
 
 
-# Standard
-import argparse
-
-# Third-Party
-import pydantic
-
 # Typing
 from typing import Optional
 
 # Local
 from pydantic_argparse import utils
 from pydantic_argparse.argparse import actions
+from pydantic_argparse.compatibility import argparse
+from pydantic_argparse.compatibility import pydantic
 
 
 def should_parse(field: pydantic.fields.ModelField) -> bool:
     """Checks whether the field should be parsed as a `boolean`.
 
     Args:
         field (pydantic.fields.ModelField): Field to check.
```

### Comparing `pydantic_argparse-0.8.0/pydantic_argparse/parsers/command.py` & `pydantic_argparse-0.9.0/src/pydantic_argparse/parsers/enum.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,58 +1,79 @@
-"""Parses Nested Pydantic Model Fields to Sub-Commands.
+"""Parses Enum Pydantic Fields to Command-Line Arguments.
 
-The `command` module contains the `should_parse` function, which checks whether
+The `enum` module contains the `should_parse` function, which checks whether
 this module should be used to parse the field, as well as the `parse_field`
-function, which parses nested `pydantic` model fields to `ArgumentParser`
-sub-commands.
+function, which parses enum `pydantic` model fields to `ArgumentParser`
+command-line arguments.
 """
 
 
 # Standard
-import argparse
-
-# Third-Party
-import pydantic
-
-# Typing
-from typing import Optional
+import enum
 
 # Local
 from pydantic_argparse import utils
+from pydantic_argparse.compatibility import argparse
+from pydantic_argparse.compatibility import pydantic
+
+# Typing
+from typing import Optional, Type
 
 
 def should_parse(field: pydantic.fields.ModelField) -> bool:
-    """Checks whether the field should be parsed as a `command`.
+    """Checks whether the field should be parsed as an `enum`.
 
     Args:
         field (pydantic.fields.ModelField): Field to check.
 
     Returns:
-        bool: Whether the field should be parsed as a `command`.
+        bool: Whether the field should be parsed as an `enum`.
     """
     # Check and Return
-    return utils.types.is_field_a(field, pydantic.BaseModel)
+    return utils.types.is_field_a(field, enum.Enum)
 
 
 def parse_field(
-    subparser: argparse._SubParsersAction,
+    parser: argparse.ArgumentParser,
     field: pydantic.fields.ModelField,
 ) -> Optional[utils.pydantic.PydanticValidator]:
-    """Adds command pydantic field to argument parser.
+    """Adds enum pydantic field to argument parser.
 
     Args:
-        subparser (argparse._SubParsersAction): Sub-parser to add to.
+        parser (argparse.ArgumentParser): Argument parser to add to.
         field (pydantic.fields.ModelField): Field to be added to parser.
 
     Returns:
         Optional[utils.pydantic.PydanticValidator]: Possible validator method.
     """
-    # Add Command
-    subparser.add_parser(
-        field.alias,
-        help=field.field_info.description,
-        model=field.outer_type_,  # type: ignore[call-arg]
-        exit_on_error=False,  # Allow top level parser to handle exiting
+    # Extract Enum
+    enum_type: Type[enum.Enum] = field.outer_type_
+
+    # Compute Argument Intrinsics
+    is_flag = len(enum_type) == 1 and not bool(field.required)
+    is_inverted = is_flag and field.get_default() is not None and field.allow_none
+
+    # Determine Argument Properties
+    metavar = f"{{{', '.join(e.name for e in enum_type)}}}"
+    action = (
+        argparse._StoreConstAction if is_flag
+        else argparse._StoreAction
+    )
+    const = (
+        {} if not is_flag
+        else {"const": None} if is_inverted
+        else {"const": next(iter(enum_type))}  # type: ignore[dict-item]
+    )
+
+    # Add Enum Field
+    parser.add_argument(
+        utils.arguments.name(field, is_inverted),
+        action=action,
+        help=utils.arguments.description(field),
+        dest=field.alias,
+        metavar=metavar,
+        required=bool(field.required),
+        **const,  # type: ignore[arg-type]
     )
 
-    # Return
-    return None
+    # Construct and Return Validator
+    return utils.pydantic.as_validator(field, lambda v: enum_type[v])
```

### Comparing `pydantic_argparse-0.8.0/pydantic_argparse/parsers/container.py` & `pydantic_argparse-0.9.0/src/pydantic_argparse/parsers/container.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,26 +4,24 @@
 whether this module should be used to parse the field, as well as the
 `parse_field` function, which parses container `pydantic` model fields to
 `ArgumentParser` command-line arguments.
 """
 
 
 # Standard
-import argparse
 import collections.abc
 import enum
 
-# Third-Party
-import pydantic
-
 # Typing
 from typing import Optional
 
 # Local
 from pydantic_argparse import utils
+from pydantic_argparse.compatibility import argparse
+from pydantic_argparse.compatibility import pydantic
 
 
 def should_parse(field: pydantic.fields.ModelField) -> bool:
     """Checks whether the field should be parsed as a `container`.
 
     Args:
         field (pydantic.fields.ModelField): Field to check.
```

### Comparing `pydantic_argparse-0.8.0/pydantic_argparse/parsers/enum.py` & `pydantic_argparse-0.9.0/src/pydantic_argparse/parsers/literal.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,41 +1,36 @@
-"""Parses Enum Pydantic Fields to Command-Line Arguments.
+"""Parses Literal Pydantic Fields to Command-Line Arguments.
 
-The `enum` module contains the `should_parse` function, which checks whether
+The `literal` module contains the `should_parse` function, which checks whether
 this module should be used to parse the field, as well as the `parse_field`
-function, which parses enum `pydantic` model fields to `ArgumentParser`
+function, which parses literal `pydantic` model fields to `ArgumentParser`
 command-line arguments.
 """
 
 
-# Standard
-import argparse
-import enum
-
-# Third-Party
-import pydantic
-
 # Local
 from pydantic_argparse import utils
+from pydantic_argparse.compatibility import argparse
+from pydantic_argparse.compatibility import pydantic
 
 # Typing
-from typing import Optional, Type
+from typing import Optional, Literal, get_args
 
 
 def should_parse(field: pydantic.fields.ModelField) -> bool:
-    """Checks whether the field should be parsed as an `enum`.
+    """Checks whether the field should be parsed as a `literal`.
 
     Args:
         field (pydantic.fields.ModelField): Field to check.
 
     Returns:
-        bool: Whether the field should be parsed as an `enum`.
+        bool: Whether the field should be parsed as a `literal`.
     """
     # Check and Return
-    return utils.types.is_field_a(field, enum.Enum)
+    return utils.types.is_field_a(field, Literal)
 
 
 def parse_field(
     parser: argparse.ArgumentParser,
     field: pydantic.fields.ModelField,
 ) -> Optional[utils.pydantic.PydanticValidator]:
     """Adds enum pydantic field to argument parser.
@@ -43,39 +38,43 @@
     Args:
         parser (argparse.ArgumentParser): Argument parser to add to.
         field (pydantic.fields.ModelField): Field to be added to parser.
 
     Returns:
         Optional[utils.pydantic.PydanticValidator]: Possible validator method.
     """
-    # Extract Enum
-    enum_type: Type[enum.Enum] = field.outer_type_
+    # Extract Choices
+    choices = get_args(field.outer_type_)
 
     # Compute Argument Intrinsics
-    is_flag = len(enum_type) == 1 and not bool(field.required)
+    is_flag = len(choices) == 1 and not bool(field.required)
     is_inverted = is_flag and field.get_default() is not None and field.allow_none
 
     # Determine Argument Properties
-    metavar = f"{{{', '.join(e.name for e in enum_type)}}}"
+    metavar = f"{{{', '.join(str(c) for c in choices)}}}"
     action = (
         argparse._StoreConstAction if is_flag
         else argparse._StoreAction
     )
     const = (
         {} if not is_flag
         else {"const": None} if is_inverted
-        else {"const": list(enum_type)[0]}
+        else {"const": choices[0]}
     )
 
-    # Add Enum Field
+    # Add Literal Field
     parser.add_argument(
         utils.arguments.name(field, is_inverted),
         action=action,
         help=utils.arguments.description(field),
         dest=field.alias,
         metavar=metavar,
         required=bool(field.required),
         **const,  # type: ignore[arg-type]
     )
 
+    # Construct String Representation Mapping of Choices
+    # This allows us O(1) parsing of choices from strings
+    mapping = {str(choice): choice for choice in choices}
+
     # Construct and Return Validator
-    return utils.pydantic.as_validator(field, lambda v: enum_type[v])
+    return utils.pydantic.as_validator(field, lambda v: mapping[v])
```

### Comparing `pydantic_argparse-0.8.0/pydantic_argparse/parsers/mapping.py` & `pydantic_argparse-0.9.0/src/pydantic_argparse/parsers/mapping.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,26 +4,24 @@
 this module should be used to parse the field, as well as the `parse_field`
 function, which parses mapping `pydantic` model fields to `ArgumentParser`
 command-line arguments.
 """
 
 
 # Standard
-import argparse
 import ast
 import collections.abc
 
-# Third-Party
-import pydantic
-
 # Typing
 from typing import Optional
 
 # Local
 from pydantic_argparse import utils
+from pydantic_argparse.compatibility import argparse
+from pydantic_argparse.compatibility import pydantic
 
 
 def should_parse(field: pydantic.fields.ModelField) -> bool:
     """Checks whether the field should be parsed as a `mapping`.
 
     Args:
         field (pydantic.fields.ModelField): Field to check.
```

### Comparing `pydantic_argparse-0.8.0/pydantic_argparse/parsers/standard.py` & `pydantic_argparse-0.9.0/src/pydantic_argparse/parsers/standard.py`

 * *Files 17% similar despite different names*

```diff
@@ -5,25 +5,21 @@
 
 Unlike the other `parser` modules, the `standard` module does not contain a
 `should_parse` function. This is because it is the fallback case, where fields
 that do not match any other types and require no special handling are parsed.
 """
 
 
-# Standard
-import argparse
-
-# Third-Party
-import pydantic
-
 # Typing
 from typing import Optional
 
 # Local
 from pydantic_argparse import utils
+from pydantic_argparse.compatibility import argparse
+from pydantic_argparse.compatibility import pydantic
 
 
 def parse_field(
     parser: argparse.ArgumentParser,
     field: pydantic.fields.ModelField,
 ) -> Optional[utils.pydantic.PydanticValidator]:
     """Adds standard pydantic field to argument parser.
```

### Comparing `pydantic_argparse-0.8.0/pydantic_argparse/utils/__init__.py` & `pydantic_argparse-0.9.0/src/pydantic_argparse/utils/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,12 +7,12 @@
 `pydantic` fields.
 
 The public interface exposed by this package is the various described utility
 modules each containing helper functions.
 """
 
 # Local
-from pydantic_argparse.utils import arguments
-from pydantic_argparse.utils import errors
-from pydantic_argparse.utils import namespaces
-from pydantic_argparse.utils import pydantic
-from pydantic_argparse.utils import types
+from pydantic_argparse.utils import arguments as arguments
+from pydantic_argparse.utils import errors as errors
+from pydantic_argparse.utils import namespaces as namespaces
+from pydantic_argparse.utils import pydantic as pydantic
+from pydantic_argparse.utils import types as types
```

### Comparing `pydantic_argparse-0.8.0/pydantic_argparse/utils/arguments.py` & `pydantic_argparse-0.9.0/src/pydantic_argparse/utils/arguments.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """Arguments Utility Functions for Declarative Typed Argument Parsing.
 
 The `arguments` module contains utility functions used for formatting argument
 names and formatting argument descriptions.
 """
 
 
-# Third-Party
-import pydantic
+# Local
+from pydantic_argparse.compatibility import pydantic
 
 
 def name(field: pydantic.fields.ModelField, invert: bool = False) -> str:
     """Standardises argument name.
 
     Args:
         field (pydantic.fields.ModelField): Field to construct name for.
```

### Comparing `pydantic_argparse-0.8.0/pydantic_argparse/utils/errors.py` & `pydantic_argparse-0.9.0/src/pydantic_argparse/utils/errors.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """Errors Utility Functions for Declarative Typed Argument Parsing.
 
 The `errors` module contains a utility function used for formatting `pydantic`
 Validation Errors to human readable messages.
 """
 
 
-# Third-Party
-import pydantic
+# Local
+from pydantic_argparse.compatibility import pydantic
 
 # Typing
 from typing import Union
 
 
 # Constants
 PydanticError = Union[pydantic.ValidationError, pydantic.env_settings.SettingsError]
```

### Comparing `pydantic_argparse-0.8.0/pydantic_argparse/utils/namespaces.py` & `pydantic_argparse-0.9.0/src/pydantic_argparse/utils/namespaces.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """Namespaces Utility Functions for Declarative Typed Argument Parsing.
 
 The `namespaces` module contains a utility function used for recursively
 converting `argparse.Namespace`s to regular Python `dict`s.
 """
 
 
-# Standard
-import argparse
+# Local
+from pydantic_argparse.compatibility import argparse
 
 # Typing
 from typing import Any, Dict
 
 
 def to_dict(namespace: argparse.Namespace) -> Dict[str, Any]:
     """Converts a nested namespace to a dictionary recursively.
```

### Comparing `pydantic_argparse-0.8.0/pydantic_argparse/utils/pydantic.py` & `pydantic_argparse-0.9.0/src/pydantic_argparse/utils/pydantic.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 dynamically generated validators and environment variable parsers.
 """
 
 
 # Standard
 import contextlib
 
-# Third-Party
-import pydantic
+# Local
+from pydantic_argparse.compatibility import pydantic
 
 # Typing
 from typing import Any, Callable, Dict, Optional, Type, TypeVar, Union
 
 
 # Constants
 T = TypeVar("T")
@@ -91,15 +91,15 @@
 
 def model_with_validators(
     model: Type[PydanticModelT],
     validators: Dict[str, PydanticValidator],
 ) -> Type[PydanticModelT]:
     """Generates a new `pydantic` model class with the supplied validators.
 
-    If the supplied base model is a subclass of `pydantic.BaseSettings`, then 
+    If the supplied base model is a subclass of `pydantic.BaseSettings`, then
     the newly generated model will also have a new `parse_env_var` classmethod
     monkeypatched onto it that suppresses any exceptions raised when initially
     parsing the environment variables. This allows the raw values to still be
     passed through to the `pydantic` field validators if initial parsing fails.
 
     Args:
         model (Type[PydanticModelT]): Model type to use as base class.
@@ -126,11 +126,11 @@
         # methods if they cannot be parsed initially.
         def __parse_env_var(field_name: str, raw_val: str) -> Any:
             with contextlib.suppress(Exception):
                 return parse_env_var(field_name, raw_val)
             return raw_val
 
         # Monkeypatch `parse_env_var`
-        model.__config__.parse_env_var = __parse_env_var  # type: ignore[assignment]
+        model.__config__.parse_env_var = __parse_env_var  # type: ignore[method-assign]
 
     # Return Constructed Model
     return model
```

### Comparing `pydantic_argparse-0.8.0/pydantic_argparse/utils/types.py` & `pydantic_argparse-0.9.0/src/pydantic_argparse/utils/types.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,28 +1,19 @@
 """Types Utility Functions for Declarative Typed Argument Parsing.
 
 The `types` module contains a utility function used for determining and
 comparing the types of `pydantic fields.
 """
 
 
-# Standard
-import sys
-
-# Third-Party
-import pydantic
+# Local
+from pydantic_argparse.compatibility import pydantic
 
 # Typing
-from typing import Any, Tuple, Union
-
-# Version-Guarded
-if sys.version_info < (3, 8):  # pragma: <3.8 cover
-    from typing_extensions import get_origin
-else:  # pragma: >=3.8 cover
-    from typing import get_origin
+from typing import Any, Tuple, Union, get_origin
 
 
 def is_field_a(
     field: pydantic.fields.ModelField,
     types: Union[Any, Tuple[Any, ...]],
 ) -> bool:
     """Checks whether the subject *is* any of the supplied types.
```

### Comparing `pydantic_argparse-0.8.0/pyproject.toml` & `pydantic_argparse-0.9.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,105 +1,113 @@
-[tool.poetry]
+[build-system]
+requires = ["hatchling", "hatch-vcs"]
+build-backend = "hatchling.build"
+
+[project]
 name = "pydantic-argparse"
-version = "0.8.0"
 description = "Typed Argument Parsing with Pydantic"
-authors = ["Hayden Richards <SupImDos@gmail.com>"]
+authors = [{ name = "Hayden Richards", email = "supimdos@gmail.com" }]
 readme = "README.md"
-license = "MIT"
-homepage = "https://pydantic-argparse.supimdos.com"
-repository = "https://github.com/SupImDos/pydantic-argparse"
-keywords = [
-    "python",
-    "pydantic",
-    "argparse",
-    "typed",
-    "validation",
+license = { file = "LICENSE" }
+requires-python = ">=3.8"
+dependencies = ["pydantic"]
+classifiers = [
+    "Development Status :: 4 - Beta",
+    'Programming Language :: Python',
+    'Programming Language :: Python :: 3',
+    'Programming Language :: Python :: 3.8',
+    'Programming Language :: Python :: 3.9',
+    'Programming Language :: Python :: 3.10',
+    'Programming Language :: Python :: 3.11',
+    'Programming Language :: Python :: 3.12',
+    'Intended Audience :: Developers',
+    'License :: OSI Approved :: MIT License',
+    'Framework :: Pydantic',
+    'Topic :: Software Development :: Libraries :: Python Modules',
 ]
-include = [
-    "LICENSE.md",
+keywords = ["python", "pydantic", "argparse", "typed", "validation"]
+dynamic = ["version"]
+
+[project.urls]
+Homepage = "https://pydantic-argparse.supimdos.com"
+Documentation = "https://pydantic-argparse.supimdos.com"
+Changelog = "https://github.com/SupImDos/pydantic-argparse/blob/master/CHANGELOG.md"
+Repository = "https://github.com/SupImDos/pydantic-argparse"
+Issues = "https://github.com/SupImDos/pydantic-argparse/issues"
+
+[tool.hatch]
+version.source = "vcs"
+build.hooks.vcs.version-file = "src/pydantic_argparse/__metadata__.py"
+build.targets.sdist.include = ["src/*", "LICENSE"]
+
+[tool.hatch.envs.default]
+installer = "uv"
+path = ".venv"
+dependencies = [
+    # Linting
+    "ruff",
+    # Typing
+    "mypy",
+    # Tests
+    "pytest",
+    "pytest-cov",
+    "pytest-mock",
+    "covdefaults",
+    # Docs
+    "mkdocs-material",
+    "mkdocstrings[python-legacy]",
+    "mkdocs-gen-files",
+    "mkdocs-literate-nav",
+    "mkdocs-autorefs",
+    # Build
+    "build",
+    "hatch",
 ]
 
-[tool.poetry.dependencies]
-python = "^3.7"
-pydantic = "^1.9.0"
-importlib_metadata = { version = ">=4", python = "<3.8" }
-typing_extensions = { version = ">=4", python = "<3.8" }
-
-[tool.poetry.group.dev.dependencies]
-poethepoet = "^0.18.1"
-mypy = "^1.0.0"
-ruff = "^0.0.247"
-pytest = "^7.2.1"
-pytest-cov = "^4.0.0"
-pytest-mock = "^3.10.0"
-covdefaults = "^2.2.2"
-mkdocs-material = "^9.0.13"
-mkdocstrings = { extras = ["python-legacy"], version = "^0.20.0" }
-mkdocs-gen-files = "^0.4.0"
-mkdocs-literate-nav = "^0.6.0"
-mkdocs-autorefs = "^0.4.1"
-
-[tool.poe.tasks]
-test = "pytest tests --cov=pydantic_argparse"
-type = "mypy tests docs pydantic_argparse"
-lint = "ruff tests docs pydantic_argparse"
-clean = "rm -rf **/.coverage **/.mypy_cache **/.pytest_cache **/.ruff_cache **/__pycache__"
-build = "poetry build"
-publish = "poetry publish"
+[tool.hatch.envs.default.scripts]
+lint = "ruff check tests docs src"
+type = "mypy tests docs src"
+test = "pytest tests --cov=src"
+build = "hatch build"
+publish = "hatch publish"
 docs-serve = "mkdocs serve"
 docs-publish = "mkdocs gh-deploy --force"
 
 [tool.ruff]
 line-length = 120
-select = [
+lint.select = [
     "F",    # flake8
     "E",    # pycodestyle errors
     "W",    # pycodestyle warnings
     "S",    # flake8-bandit
     "B",    # flake8-bugbear
     "A",    # flake8-builtins
     "D",    # flake8-docstrings
     "PT",   # flake8-pytest-style
     "Q",    # flake8-quotes
     "RUF",  # ruff
 ]
-ignore = [
-    "D401"  # imperative mood - overly restrictive
+lint.ignore = [
+    "D401",  # imperative mood - overly restrictive
+    "S101",  # allow assertions
 ]
-
-[tool.ruff.per-file-ignores]
-"__init__.py" = ["F401"]  # allow unused imports in `__init__.py`
-"tests/*.py" = ["S101"]   # allow asserts in unit tests
-
-[tool.ruff.pydocstyle]
-convention = "google"
-
-[tool.pytest.ini_options]
-addopts = "--verbose"
-log_cli_level = "DEBUG"
-log_cli_format = "%(asctime)s.%(msecs)03d [%(levelname)-8s] (%(name)-11s): %(message)s"
-log_cli_date_format = "%Y%m%dT%H%M%S"
-
-[tool.coverage.run]
-plugins = ["covdefaults"]
+lint.pydocstyle = { convention = "google" }
 
 [tool.mypy]
 check_untyped_defs = true
 disallow_untyped_defs = true
 disallow_incomplete_defs = true
 disallow_untyped_decorators = true
 disallow_any_unimported = true
 warn_return_any = true
 warn_unused_ignores = true
 no_implicit_optional = true
 show_error_codes = true
-plugins = ["pydantic.mypy"]
+plugins = ["pydantic.v1.mypy"]
 
 [tool.pydantic-mypy]
 init_forbid_extra = true
 init_typed = true
 warn_required_dynamic_aliases = true
-warn_untyped_fields = true
 
-[build-system]
-requires = ["poetry-core"]
-build-backend = "poetry.core.masonry.api"
+[tool.coverage.run]
+plugins = ["covdefaults"]
```

### Comparing `pydantic_argparse-0.8.0/PKG-INFO` & `pydantic_argparse-0.9.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,28 +1,54 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: pydantic-argparse
-Version: 0.8.0
+Version: 0.9.0
 Summary: Typed Argument Parsing with Pydantic
-Home-page: https://pydantic-argparse.supimdos.com
-License: MIT
-Keywords: python,pydantic,argparse,typed,validation
-Author: Hayden Richards
-Author-email: SupImDos@gmail.com
-Requires-Python: >=3.7,<4.0
+Project-URL: Homepage, https://pydantic-argparse.supimdos.com
+Project-URL: Documentation, https://pydantic-argparse.supimdos.com
+Project-URL: Changelog, https://github.com/SupImDos/pydantic-argparse/blob/master/CHANGELOG.md
+Project-URL: Repository, https://github.com/SupImDos/pydantic-argparse
+Project-URL: Issues, https://github.com/SupImDos/pydantic-argparse/issues
+Author-email: Hayden Richards <supimdos@gmail.com>
+License: MIT License
+        
+        Copyright (c) 2021 Hayden Richards
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy
+        of this software and associated documentation files (the "Software"), to deal
+        in the Software without restriction, including without limitation the rights
+        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+        copies of the Software, and to permit persons to whom the Software is
+        furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in all
+        copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+        SOFTWARE.
+License-File: LICENSE
+Keywords: argparse,pydantic,python,typed,validation
+Classifier: Development Status :: 4 - Beta
+Classifier: Framework :: Pydantic
+Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: importlib_metadata (>=4) ; python_version < "3.8"
-Requires-Dist: pydantic (>=1.9.0,<2.0.0)
-Requires-Dist: typing_extensions (>=4) ; python_version < "3.8"
-Project-URL: Repository, https://github.com/SupImDos/pydantic-argparse
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Python: >=3.8
+Requires-Dist: pydantic
 Description-Content-Type: text/markdown
 
 <div align="center">
     <a href="https://pydantic-argparse.supimdos.com">
         <img src="https://raw.githubusercontent.com/SupImDos/pydantic-argparse/master/docs/assets/images/logo.svg" width="50%">
     </a>
     <h1>
@@ -57,23 +83,26 @@
         <img src="https://img.shields.io/github/actions/workflow/status/supimdos/pydantic-argparse/typing.yml?label=typing">
     </a>
 </div>
 
 ## Help
 See [documentation](https://pydantic-argparse.supimdos.com) for help.
 
+## Requirements
+Requires Python 3.8+, and is compatible with the Pydantic v1 API.
+
 ## Installation
 Installation with `pip` is simple:
 ```console
 $ pip install pydantic-argparse
 ```
 
 ## Example
 ```py
-import pydantic
+import pydantic.v1 as pydantic
 import pydantic_argparse
 
 
 class Arguments(pydantic.BaseModel):
     # Required Args
     string: str = pydantic.Field(description="a required string")
     integer: int = pydantic.Field(description="a required integer")
@@ -129,8 +158,7 @@
 ```console
 $ python3 example.py --string hello --integer 42 --flag
 string='hello' integer=42 flag=True second_flag=False third_flag=True
 ```
 
 ## License
 This project is licensed under the terms of the MIT license.
-
```

