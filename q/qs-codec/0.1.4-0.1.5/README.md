# Comparing `tmp/qs_codec-0.1.4.tar.gz` & `tmp/qs_codec-0.1.5.tar.gz`

## Comparing `qs_codec-0.1.4.tar` & `qs_codec-0.1.5.tar`

### file list

```diff
@@ -1,44 +1,44 @@
--rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 qs_codec-0.1.4/CHANGELOG.md
--rw-r--r--   0        0        0     5513 2020-02-02 00:00:00.000000 qs_codec-0.1.4/CODE-OF-CONDUCT.md
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 qs_codec-0.1.4/requirements_dev.txt
--rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 qs_codec-0.1.4/src/qs_codec/__init__.py
--rw-r--r--   0        0        0     6654 2020-02-02 00:00:00.000000 qs_codec-0.1.4/src/qs_codec/decode.py
--rw-r--r--   0        0        0    10345 2020-02-02 00:00:00.000000 qs_codec-0.1.4/src/qs_codec/encode.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qs_codec-0.1.4/src/qs_codec/py.typed
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qs_codec-0.1.4/src/qs_codec/enums/__init__.py
--rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 qs_codec-0.1.4/src/qs_codec/enums/charset.py
--rw-r--r--   0        0        0      415 2020-02-02 00:00:00.000000 qs_codec-0.1.4/src/qs_codec/enums/duplicates.py
--rw-r--r--   0        0        0      921 2020-02-02 00:00:00.000000 qs_codec-0.1.4/src/qs_codec/enums/format.py
--rw-r--r--   0        0        0     1733 2020-02-02 00:00:00.000000 qs_codec-0.1.4/src/qs_codec/enums/list_format.py
--rw-r--r--   0        0        0      950 2020-02-02 00:00:00.000000 qs_codec-0.1.4/src/qs_codec/enums/sentinel.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qs_codec-0.1.4/src/qs_codec/models/__init__.py
--rw-r--r--   0        0        0     4350 2020-02-02 00:00:00.000000 qs_codec-0.1.4/src/qs_codec/models/decode_options.py
--rw-r--r--   0        0        0     5151 2020-02-02 00:00:00.000000 qs_codec-0.1.4/src/qs_codec/models/encode_options.py
--rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 qs_codec-0.1.4/src/qs_codec/models/undefined.py
--rw-r--r--   0        0        0     1254 2020-02-02 00:00:00.000000 qs_codec-0.1.4/src/qs_codec/models/weak_wrapper.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qs_codec-0.1.4/src/qs_codec/utils/__init__.py
--rw-r--r--   0        0        0     1711 2020-02-02 00:00:00.000000 qs_codec-0.1.4/src/qs_codec/utils/decode_utils.py
--rw-r--r--   0        0        0     4880 2020-02-02 00:00:00.000000 qs_codec-0.1.4/src/qs_codec/utils/encode_utils.py
--rw-r--r--   0        0        0      762 2020-02-02 00:00:00.000000 qs_codec-0.1.4/src/qs_codec/utils/str_utils.py
--rw-r--r--   0        0        0     8571 2020-02-02 00:00:00.000000 qs_codec-0.1.4/src/qs_codec/utils/utils.py
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 qs_codec-0.1.4/tests/comparison/.gitignore
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qs_codec-0.1.4/tests/comparison/__init__.py
--rwxr-xr-x   0        0        0      408 2020-02-02 00:00:00.000000 qs_codec-0.1.4/tests/comparison/compare_outputs.sh
--rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 qs_codec-0.1.4/tests/comparison/package.json
--rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 qs_codec-0.1.4/tests/comparison/qs.js
--rw-r--r--   0        0        0      929 2020-02-02 00:00:00.000000 qs_codec-0.1.4/tests/comparison/qs.py
--rw-r--r--   0        0        0     1204 2020-02-02 00:00:00.000000 qs_codec-0.1.4/tests/comparison/test_cases.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qs_codec-0.1.4/tests/e2e/__init__.py
--rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 qs_codec-0.1.4/tests/e2e/e2e_test.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qs_codec-0.1.4/tests/unit/__init__.py
--rw-r--r--   0        0        0    29989 2020-02-02 00:00:00.000000 qs_codec-0.1.4/tests/unit/decode_test.py
--rw-r--r--   0        0        0    50930 2020-02-02 00:00:00.000000 qs_codec-0.1.4/tests/unit/encode_test.py
--rw-r--r--   0        0        0    22214 2020-02-02 00:00:00.000000 qs_codec-0.1.4/tests/unit/example_test.py
--rw-r--r--   0        0        0      503 2020-02-02 00:00:00.000000 qs_codec-0.1.4/tests/unit/fixed_qs_issues_test.py
--rw-r--r--   0        0        0    14896 2020-02-02 00:00:00.000000 qs_codec-0.1.4/tests/unit/utils_test.py
--rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 qs_codec-0.1.4/tests/unit/weakref_test.py
--rw-r--r--   0        0        0     1343 2020-02-02 00:00:00.000000 qs_codec-0.1.4/.gitignore
--rw-r--r--   0        0        0     1498 2020-02-02 00:00:00.000000 qs_codec-0.1.4/LICENSE
--rw-r--r--   0        0        0    24736 2020-02-02 00:00:00.000000 qs_codec-0.1.4/README.md
--rw-r--r--   0        0        0     2698 2020-02-02 00:00:00.000000 qs_codec-0.1.4/pyproject.toml
--rw-r--r--   0        0        0    26220 2020-02-02 00:00:00.000000 qs_codec-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 qs_codec-0.1.5/CHANGELOG.md
+-rw-r--r--   0        0        0     5513 2020-02-02 00:00:00.000000 qs_codec-0.1.5/CODE-OF-CONDUCT.md
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 qs_codec-0.1.5/requirements_dev.txt
+-rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 qs_codec-0.1.5/src/qs_codec/__init__.py
+-rw-r--r--   0        0        0     6715 2020-02-02 00:00:00.000000 qs_codec-0.1.5/src/qs_codec/decode.py
+-rw-r--r--   0        0        0    10374 2020-02-02 00:00:00.000000 qs_codec-0.1.5/src/qs_codec/encode.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qs_codec-0.1.5/src/qs_codec/py.typed
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qs_codec-0.1.5/src/qs_codec/enums/__init__.py
+-rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 qs_codec-0.1.5/src/qs_codec/enums/charset.py
+-rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 qs_codec-0.1.5/src/qs_codec/enums/duplicates.py
+-rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 qs_codec-0.1.5/src/qs_codec/enums/format.py
+-rw-r--r--   0        0        0     1759 2020-02-02 00:00:00.000000 qs_codec-0.1.5/src/qs_codec/enums/list_format.py
+-rw-r--r--   0        0        0      982 2020-02-02 00:00:00.000000 qs_codec-0.1.5/src/qs_codec/enums/sentinel.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qs_codec-0.1.5/src/qs_codec/models/__init__.py
+-rw-r--r--   0        0        0     4548 2020-02-02 00:00:00.000000 qs_codec-0.1.5/src/qs_codec/models/decode_options.py
+-rw-r--r--   0        0        0     5297 2020-02-02 00:00:00.000000 qs_codec-0.1.5/src/qs_codec/models/encode_options.py
+-rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 qs_codec-0.1.5/src/qs_codec/models/undefined.py
+-rw-r--r--   0        0        0     1254 2020-02-02 00:00:00.000000 qs_codec-0.1.5/src/qs_codec/models/weak_wrapper.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qs_codec-0.1.5/src/qs_codec/utils/__init__.py
+-rw-r--r--   0        0        0     1711 2020-02-02 00:00:00.000000 qs_codec-0.1.5/src/qs_codec/utils/decode_utils.py
+-rw-r--r--   0        0        0     4884 2020-02-02 00:00:00.000000 qs_codec-0.1.5/src/qs_codec/utils/encode_utils.py
+-rw-r--r--   0        0        0      762 2020-02-02 00:00:00.000000 qs_codec-0.1.5/src/qs_codec/utils/str_utils.py
+-rw-r--r--   0        0        0     8575 2020-02-02 00:00:00.000000 qs_codec-0.1.5/src/qs_codec/utils/utils.py
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 qs_codec-0.1.5/tests/comparison/.gitignore
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qs_codec-0.1.5/tests/comparison/__init__.py
+-rwxr-xr-x   0        0        0      408 2020-02-02 00:00:00.000000 qs_codec-0.1.5/tests/comparison/compare_outputs.sh
+-rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 qs_codec-0.1.5/tests/comparison/package.json
+-rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 qs_codec-0.1.5/tests/comparison/qs.js
+-rw-r--r--   0        0        0      929 2020-02-02 00:00:00.000000 qs_codec-0.1.5/tests/comparison/qs.py
+-rw-r--r--   0        0        0     1204 2020-02-02 00:00:00.000000 qs_codec-0.1.5/tests/comparison/test_cases.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qs_codec-0.1.5/tests/e2e/__init__.py
+-rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 qs_codec-0.1.5/tests/e2e/e2e_test.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qs_codec-0.1.5/tests/unit/__init__.py
+-rw-r--r--   0        0        0    29989 2020-02-02 00:00:00.000000 qs_codec-0.1.5/tests/unit/decode_test.py
+-rw-r--r--   0        0        0    50930 2020-02-02 00:00:00.000000 qs_codec-0.1.5/tests/unit/encode_test.py
+-rw-r--r--   0        0        0    22214 2020-02-02 00:00:00.000000 qs_codec-0.1.5/tests/unit/example_test.py
+-rw-r--r--   0        0        0      503 2020-02-02 00:00:00.000000 qs_codec-0.1.5/tests/unit/fixed_qs_issues_test.py
+-rw-r--r--   0        0        0    14896 2020-02-02 00:00:00.000000 qs_codec-0.1.5/tests/unit/utils_test.py
+-rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 qs_codec-0.1.5/tests/unit/weakref_test.py
+-rw-r--r--   0        0        0     1343 2020-02-02 00:00:00.000000 qs_codec-0.1.5/.gitignore
+-rw-r--r--   0        0        0     1498 2020-02-02 00:00:00.000000 qs_codec-0.1.5/LICENSE
+-rw-r--r--   0        0        0    24623 2020-02-02 00:00:00.000000 qs_codec-0.1.5/README.md
+-rw-r--r--   0        0        0     2753 2020-02-02 00:00:00.000000 qs_codec-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0    26107 2020-02-02 00:00:00.000000 qs_codec-0.1.5/PKG-INFO
```

### Comparing `qs_codec-0.1.4/CODE-OF-CONDUCT.md` & `qs_codec-0.1.5/CODE-OF-CONDUCT.md`

 * *Files identical despite different names*

### Comparing `qs_codec-0.1.4/src/qs_codec/decode.py` & `qs_codec-0.1.5/src/qs_codec/decode.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,19 @@
 from .enums.sentinel import Sentinel
 from .models.decode_options import DecodeOptions
 from .models.undefined import Undefined
 from .utils.utils import Utils
 
 
 def decode(value: t.Optional[t.Union[str, t.Mapping]], options: DecodeOptions = DecodeOptions()) -> dict:
-    """Decodes a str or Mapping into a Dict. Providing custom DecodeOptions will override the default behavior."""
+    """
+    Decodes a ``str`` or ``Mapping`` into a ``dict``.
+
+    Providing custom ``DecodeOptions`` will override the default behavior.
+    """
     if not value:
         return dict()
 
     if not isinstance(value, (str, t.Mapping)):
         raise ValueError("The input must be a String or a Dict")
 
     temp_obj: t.Optional[t.Mapping] = _parse_query_string_values(value, options) if isinstance(value, str) else value
@@ -103,15 +107,17 @@
             obj[key] = Utils.combine(obj[key], val)
         elif not existing or options.duplicates == Duplicates.LAST:
             obj[key] = val
 
     return obj
 
 
-def _parse_object(chain: t.Sequence[str], val: t.Any, options: DecodeOptions, values_parsed: bool) -> t.Any:
+def _parse_object(
+    chain: t.Union[t.List[str], t.Tuple[str, ...]], val: t.Any, options: DecodeOptions, values_parsed: bool
+) -> t.Any:
     leaf: t.Any = val if values_parsed else _parse_array_value(val, options)
 
     i: int
     for i in reversed(range(len(chain))):
         obj: t.Optional[t.Any]
         root: str = chain[i]
```

### Comparing `qs_codec-0.1.4/src/qs_codec/encode.py` & `qs_codec-0.1.5/src/qs_codec/encode.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,19 @@
 from .models.encode_options import EncodeOptions
 from .models.undefined import Undefined
 from .models.weak_wrapper import WeakWrapper
 from .utils.utils import Utils
 
 
 def encode(value: t.Any, options: EncodeOptions = EncodeOptions()) -> str:
-    """Encodes an object into a query string. Providing custom EncodeOptions will override the default behavior."""
+    """
+    Encodes ``Any`` object into a query ``str`` ing.
+
+    Providing custom ``EncodeOptions`` will override the default behavior.
+    """
     if value is None:
         return ""
 
     obj: t.Mapping[str, t.Any]
     if isinstance(value, t.Mapping):
         obj = deepcopy(value)
     elif isinstance(value, (list, tuple)):
```

### Comparing `qs_codec-0.1.4/src/qs_codec/enums/format.py` & `qs_codec-0.1.5/src/qs_codec/enums/format.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,32 +6,32 @@
 
 
 class Formatter:
     """A class for formatting URI components."""
 
     @staticmethod
     def rfc1738(value: str) -> str:
-        """Format a string according to RFC 1738."""
+        """Format a string according to `RFC 1738 <https://datatracker.ietf.org/doc/html/rfc1738>`_."""
         return value.replace("%20", "+")
 
     @staticmethod
     def rfc3986(value: str) -> str:
-        """Format a string according to RFC 3986."""
+        """Format a string according to `RFC 3986 <https://datatracker.ietf.org/doc/html/rfc3986>`_."""
         return value
 
 
 @dataclass(frozen=True)
-class FormatDataMixin:
+class _FormatDataMixin:
     """Format data mixin."""
 
     format_name: str
     formatter: t.Callable[[str], str]
 
 
-class Format(FormatDataMixin, Enum):
+class Format(_FormatDataMixin, Enum):
     """An enum of all supported URI component encoding formats."""
 
-    # https://datatracker.ietf.org/doc/html/rfc1738
     RFC1738 = "RFC1738", Formatter.rfc1738
+    """`RFC 1738 <https://datatracker.ietf.org/doc/html/rfc1738>`_."""
 
-    # https://datatracker.ietf.org/doc/html/rfc3986
     RFC3986 = "RFC3986", Formatter.rfc3986
+    """`RFC 3986 <https://datatracker.ietf.org/doc/html/rfc3986>`_."""
```

### Comparing `qs_codec-0.1.4/src/qs_codec/enums/list_format.py` & `qs_codec-0.1.5/src/qs_codec/enums/list_format.py`

 * *Files 19% similar despite different names*

```diff
@@ -26,28 +26,28 @@
     @staticmethod
     def repeat(prefix: str, key: t.Optional[str] = None) -> str:  # pylint: disable=W0613
         """Format a list item using repeats."""
         return prefix
 
 
 @dataclass(frozen=True)
-class ListFormatDataMixin:
+class _ListFormatDataMixin:
     """List format data mixin."""
 
     list_format_name: str
     generator: t.Callable[[str, t.Optional[str]], str]
 
 
-class ListFormat(ListFormatDataMixin, Enum):
+class ListFormat(_ListFormatDataMixin, Enum):
     """An enum of all available list format options."""
 
-    # Use brackets to represent list items, for example `foo[]=123&foo[]=456&foo[]=789`
     BRACKETS = "BRACKETS", ListFormatGenerator.brackets
+    """Use brackets to represent list items, for example ``foo[]=123&foo[]=456&foo[]=789``"""
 
-    # Use commas to represent list items, for example `foo=123,456,789`
     COMMA = "COMMA", ListFormatGenerator.comma
+    """Use commas to represent list items, for example ``foo=123,456,789``"""
 
-    # Use a repeat key to represent list items, for example `foo=123&foo=456&foo=789`
     REPEAT = "REPEAT", ListFormatGenerator.repeat
+    """Use a repeat key to represent list items, for example ``foo=123&foo=456&foo=789``"""
 
-    # Use indices to represent list items, for example `foo[0]=123&foo[1]=456&foo[2]=789`
     INDICES = "INDICES", ListFormatGenerator.indices
+    """Use indices to represent list items, for example ``foo[0]=123&foo[1]=456&foo[2]=789``"""
```

### Comparing `qs_codec-0.1.4/src/qs_codec/models/decode_options.py` & `qs_codec-0.1.5/src/qs_codec/models/decode_options.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,93 +1,91 @@
-"""Options that configure the output of QS.decode."""
+"""This module contains the ``DecodeOptions`` class that configures the output of ``decode``."""
 
 import typing as t
 from dataclasses import dataclass, field
 
 from ..enums.charset import Charset
 from ..enums.duplicates import Duplicates
 from ..utils.decode_utils import DecodeUtils
 
 
 @dataclass
 class DecodeOptions:
-    """Options that configure the output of QS.decode."""
+    """Options that configure the output of ``decode``."""
 
-    # Set to `True` to decode dot `Dict` notation in the encoded input.
     allow_dots: bool = field(default=None)  # type: ignore [assignment]
+    """Set to ``True`` to decode dot ``dict`` notation in the encoded input."""
 
-    # Set to `True` to decode dots in keys.
-    # Note: it implies `allow_dots`, so `QS.decode` will error if you set decode_dot_in_keys` to `True`, and
-    # `allow_dots` to `False.
     decode_dot_in_keys: bool = field(default=None)  # type: ignore [assignment]
+    """Set to ``True`` to decode dots in keys.
+    Note: it implies ``allow_dots``, so ``decode`` will error if you set ``decode_dot_in_keys`` to ``True``, and
+    ``allow_dots`` to ``False``."""
 
-    # Set to `True` to allow empty `List` values inside `Dict`s in the encoded input
     allow_empty_lists: bool = False
+    """Set to ``True`` to allow empty ``list`` values inside ``dict``\\s in the encoded input."""
 
-    # `QS` will limit specifying indices in a `List` to a maximum index of `20`.
-    # Any `List` members with an index of greater than `20` will instead be converted to a `Dict` with the index as the
-    # key. This is needed to handle cases when someone sent, for example, `a[999999999]` and it will take significant
-    # time to iterate over this huge `List`.
-    # This limit can be overridden by passing a `list_limit` option.
     list_limit: int = 20
+    """``qs_codec`` will limit specifying indices in a ``list`` to a maximum index of ``20``.
+    Any ``list`` members with an index of greater than ``20`` will instead be converted to a ``dict`` with the index as
+    the key. This is needed to handle cases when someone sent, for example, ``a[999999999]`` and it will take
+    significant time to iterate over this huge ``list``.
+    This limit can be overridden by passing a ``list_limit`` option."""
 
-    # The character encoding to use when decoding the input.
     charset: Charset = Charset.UTF8
+    """The character encoding to use when decoding the input."""
 
-    # Some services add an initial `utf8=✓` value to forms so that old InternetExplorer versions are more likely to
-    # submit the form as `utf-8`. Additionally, the server can check the value against wrong encodings of the checkmark
-    # character and detect that a query string or `application/x-www-form-urlencoded` body was *not* sent as `utf-8`,
-    # e.g. if the form had an `accept-charset` parameter or the containing page had a different character set.
-    #
-    # `QS` supports this mechanism via the `charset_sentinel` option.
-    # If specified, the `utf-8` parameter will be omitted from the returned `Dict`.
-    # It will be used to switch to `latin-1`/`utf-8` mode depending on how the checkmark is encoded.
-    #
-    # Important: When you specify both the `charset` option and the `charset_sentinel` option,
-    # the `charset` will be overridden when the request contains a `utf-8` parameter from which the actual charset
-    # can be deduced. In that sense the `charset` will behave as the default charset rather than the authoritative
-    # charset.
     charset_sentinel: bool = False
+    """Some services add an initial ``utf8=✓`` value to forms so that old InternetExplorer versions are more likely to
+    submit the form as ``utf-8``. Additionally, the server can check the value against wrong encodings of the checkmark
+    character and detect that a query string or ``application/x-www-form-urlencoded`` body was *not* sent as ``utf-8``,
+    e.g. if the form had an ``accept-charset`` parameter or the containing page had a different character set.
+
+    ``qs_codec`` supports this mechanism via the ``charset_sentinel`` option.
+    If specified, the ``utf-8`` parameter will be omitted from the returned ``dict``.
+    It will be used to switch to ``LATIN1`` or ``UTF8`` mode depending on how the checkmark is encoded.
+
+    Important: When you specify both the ``charset`` option and the ``charset_sentinel`` option,
+    the ``charset`` will be overridden when the request contains a ``utf-8`` parameter from which the actual charset
+    can be deduced. In that sense the ``charset`` will behave as the default charset rather than the authoritative
+    charset."""
 
-    # Set to `True` to parse the input as a comma-separated value.
-    # Note: nested `Dict`s, such as `'a={b:1},{c:d}'` are not supported.
     comma: bool = False
+    """Set to ``True`` to parse the input as a comma-separated value.
+    Note: nested ``dict`` s, such as ``'a={b:1},{c:d}'`` are not supported."""
 
-    # The delimiter to use when splitting key-value pairs in the encoded input.
-    # Can be a `str` or a `Pattern`.
     delimiter: t.Union[str, t.Pattern[str]] = "&"
+    """The delimiter to use when splitting key-value pairs in the encoded input. Can be a ``str`` or a ``Pattern``."""
 
-    # By default, when nesting `Dict`s `QS` will only decode up to 5 children deep.
-    # This depth can be overridden by setting the `depth`.
-    # The depth limit helps mitigate abuse when `QS` is used to parse user input,
-    # and it is recommended to keep it a reasonably small number.
     depth: int = 5
+    """By default, when nesting ``dict``\\s ``qs_codec`` will only decode up to 5 children deep.
+    This depth can be overridden by setting the ``depth``.
+    The depth limit helps mitigate abuse when ``qs_codec`` is used to parse user input,
+    and it is recommended to keep it a reasonably small number."""
 
-    # For similar reasons, by default `QS` will only parse up to 1000
-    # parameters. This can be overridden by passing a `parameter_limit`
-    # option.
     parameter_limit: t.Union[int, float] = 1000
+    """For similar reasons, by default ``qs_codec`` will only parse up to 1000 parameters. This can be overridden by
+    passing a ``parameter_limit`` option."""
 
-    # Change the duplicate key handling strategy
     duplicates: Duplicates = Duplicates.COMBINE
+    """Change the duplicate key handling strategy."""
 
-    # Set to `True` to ignore the leading question mark query prefix in the encoded input.
     ignore_query_prefix: bool = False
+    """Set to ``True`` to ignore the leading question mark query prefix in the encoded input."""
 
-    # Set to `True` to interpret HTML numeric entities (`&#...;`) in the encoded input.
     interpret_numeric_entities: bool = False
+    """Set to ``True`` to interpret HTML numeric entities (``&#...;``) in the encoded input."""
 
-    # To disable `List` parsing entirely, set `parse_lists` to `False`.
     parse_lists: bool = True
+    """To disable ``list`` parsing entirely, set ``parse_lists`` to ``False``."""
 
-    # Set to true to decode values without `=` to `null`.
     strict_null_handling: bool = False
+    """Set to true to decode values without ``=`` to ``None``."""
 
-    # Set a decoder to affect the decoding of the input.
     decoder: t.Callable[[t.Optional[str], t.Optional[Charset]], t.Any] = DecodeUtils.decode
+    """Set a ``Callable`` to affect the decoding of the input."""
 
     def __post_init__(self):
         """Post-initialization."""
         if self.allow_dots is None:
             self.allow_dots = self.decode_dot_in_keys is True or False
         if self.decode_dot_in_keys is None:
             self.decode_dot_in_keys = False
```

### Comparing `qs_codec-0.1.4/src/qs_codec/models/encode_options.py` & `qs_codec-0.1.5/src/qs_codec/models/encode_options.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,104 +1,102 @@
-"""This module contains the `EncodeOptions` class that configures the output of QS.encode."""
+"""This module contains the ``EncodeOptions`` class that configures the output of ``encode``."""
 
 import typing as t
 from dataclasses import asdict, dataclass, field
 from datetime import datetime
 
 from ..enums.charset import Charset
 from ..enums.format import Format
 from ..enums.list_format import ListFormat
 from ..utils.encode_utils import EncodeUtils
 
 
 @dataclass
 class EncodeOptions:
-    """Options that configure the output of QS.encode."""
+    """Options that configure the output of ``encode``."""
 
-    # Set to `True` to use dot `Dict` notation in the encoded output.
     allow_dots: bool = field(default=None)  # type: ignore [assignment]
+    """Set to ``True`` to use dot ``dict`` notation in the encoded output."""
 
-    # Set to `True` to add a question mark `?` prefix to the encoded output.
     add_query_prefix: bool = False
+    """Set to ``True`` to add a question mark ``?`` prefix to the encoded output."""
 
-    # Set to `True` to allow empty `List`s in the encoded output.
     allow_empty_lists: bool = False
+    """Set to ``True`` to allow empty ``list`` s in the encoded output."""
 
-    # Deprecated: Use `list_format` instead.
     indices: t.Optional[bool] = None
+    """Deprecated: Use ``list_format`` instead."""
 
-    # The `List` encoding format to use.
     list_format: ListFormat = ListFormat.INDICES
+    """The ``list`` encoding format to use."""
 
-    # The character encoding to use.
     charset: Charset = Charset.UTF8
+    """The character encoding to use."""
 
-    # Set to `True` to announce the character by including an `utf8=✓` parameter
-    # with the proper encoding of the checkmark, similar to what Ruby on Rails
-    # and others do when submitting forms.
     charset_sentinel: bool = False
+    """Set to ``True`` to announce the character by including an ``utf8=✓`` parameter with the proper encoding of the
+    checkmark, similar to what Ruby on Rails and others do when submitting forms."""
 
-    # The delimiter to use when joining key-value pairs in the encoded output."""
     delimiter: str = "&"
+    """The delimiter to use when joining key-value pairs in the encoded output."""
 
-    # Set to `False` to disable encoding."""
     encode: bool = True
+    """Set to ``False`` to disable encoding."""
 
-    # Encode `Dict` keys using dot notation by setting `encode_dot_in_keys` to `True`
-    # Caveat: When `encode_values_only` is `True` as well as `encode_dot_in_keys`,
-    # only dots in keys and nothing else will be encoded.
     encode_dot_in_keys: bool = field(default=None)  # type: ignore [assignment]
+    """Encode ``dict`` keys using dot notation by setting ``encode_dot_in_keys`` to ``True``.
+    Caveat: When ``encode_values_only`` is ``True`` as well as ``encode_dot_in_keys``, only dots in keys and nothing
+    else will be encoded."""
 
-    # Encoding can be disabled for keys by setting the `encode_values_only` to `True`"""
     encode_values_only: bool = False
+    """Encoding can be disabled for keys by setting the ``encode_values_only`` to ``True``."""
 
-    # The encoding format to use.
-    # The default `format` is `Format.RFC3986` which encodes `' '` to `%20` which is backward compatible.
-    # You can also set `format` to `Format.RFC1738` which encodes `' '` to `+`.
     format: Format = Format.RFC3986
+    """The encoding format to use.
+    The default ``format`` is ``Format.RFC3986`` which encodes ``' '`` to ``%20`` which is backward compatible.
+    You can also set ``format`` to ``Format.RFC1738`` which encodes ``' '`` to ``+``."""
 
-    # Use the `filter` option to restrict which keys will be included in the encoded output.
-    # If you pass a `Callable`, it will be called for each key to obtain the replacement value.
-    # If you pass a `List`, it will be used to select properties and `List` indices to be encoded.
     filter: t.Optional[t.Union[t.Callable, t.List[t.Union[str, int]]]] = field(default=None)
+    """Use the ``filter`` option to restrict which keys will be included in the encoded output.
+    If you pass a ``Callable``, it will be called for each key to obtain the replacement value.
+    If you pass a ``list``, it will be used to select properties and ``list`` indices to be encoded."""
 
-    # Set to `True` to completely skip encoding keys with `null` values"""
     skip_nulls: bool = False
+    """Set to ``True`` to completely skip encoding keys with ``None`` values."""
 
-    # If you only want to override the serialization of `datetime` objects,
-    # you can provide a `Callable`.
     serialize_date: t.Callable[[datetime], str] = EncodeUtils.serialize_date
+    """If you only want to override the serialization of ``datetime`` objects, you can provide a ``Callable``."""
 
-    # Set an `Encoder` to affect the encoding of values.
-    # Note: the `encoder` option does not apply if `encode` is `False`
     encoder: t.Callable[[t.Any, t.Optional[Charset], t.Optional[Format]], str] = field(  # type: ignore [assignment]
         default_factory=EncodeUtils.encode  # type: ignore [arg-type]
     )
+    """Set an ``Encoder`` to affect the encoding of values.
+    Note: the ``encoder`` option does not apply if ``encode`` is ``False``."""
+
     _encoder: t.Callable[[t.Any, t.Optional[Charset], t.Optional[Format]], str] = field(init=False, repr=False)
 
     @property  # type: ignore [no-redef]
     def encoder(self) -> t.Callable[[t.Any, t.Optional[Charset], t.Optional[Format]], str]:  # noqa: F811
         """Get the encoder function."""
         return lambda v, c=self.charset, f=self.format: self._encoder(v, c, f)  # type: ignore [misc]
 
     @encoder.setter
     def encoder(self, value: t.Optional[t.Callable[[t.Any, t.Optional[Charset], t.Optional[Format]], str]]) -> None:
         self._encoder = value if callable(value) else EncodeUtils.encode  # type: ignore [assignment]
 
-    # Set to `True` to distinguish between `null` values and empty `str`ings.
-    # This way the encoded string `null` values will have no `=` sign.
     strict_null_handling: bool = False
+    """Set to ``True`` to distinguish between ``null`` values and empty ``str``\\ings. This way the encoded string
+    ``None`` values will have no ``=`` sign."""
 
-    # When `list_format` is set to `ListFormat.COMMA`, you can also set
-    # `comma_round_trip` option to `True` or `False`, to append `[]` on
-    # single-item `List`s, so that they can round trip through a parse.
     comma_round_trip: t.Optional[bool] = None
+    """When ``list_format`` is set to ``ListFormat.COMMA``, you can also set ``comma_round_trip`` option to ``True`` or
+    ``False``, to append ``[]`` on single-item ``list``\\s, so that they can round trip through a parse."""
 
-    # Set a `Sorter` to affect the order of parameter keys.
     sort: t.Optional[t.Callable[[t.Any, t.Any], int]] = field(default=None)
+    """Set a ``Callable`` to affect the order of parameter keys."""
 
     def __post_init__(self):
         """Post-initialization."""
         if self.allow_dots is None:
             self.allow_dots = self.encode_dot_in_keys is True or False
         if self.encode_dot_in_keys is None:
             self.encode_dot_in_keys = False
```

### Comparing `qs_codec-0.1.4/src/qs_codec/models/weak_wrapper.py` & `qs_codec-0.1.5/src/qs_codec/models/weak_wrapper.py`

 * *Files identical despite different names*

### Comparing `qs_codec-0.1.4/src/qs_codec/utils/decode_utils.py` & `qs_codec-0.1.5/src/qs_codec/utils/decode_utils.py`

 * *Files identical despite different names*

### Comparing `qs_codec-0.1.4/src/qs_codec/utils/encode_utils.py` & `qs_codec-0.1.5/src/qs_codec/utils/encode_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,16 +10,16 @@
 from ..enums.format import Format
 from .str_utils import code_unit_at
 
 
 class EncodeUtils:
     """A collection of encode utility methods used by the library."""
 
-    # Hex table of all 256 characters
     HEX_TABLE: t.Tuple[str, ...] = tuple(f"%{i.to_bytes(1, 'big').hex().upper().zfill(2)}" for i in range(256))
+    """Hex table of all 256 characters"""
 
     @classmethod
     def escape(
         cls,
         string: str,
         format: t.Optional[Format] = Format.RFC3986,
     ) -> str:
```

### Comparing `qs_codec-0.1.4/src/qs_codec/utils/str_utils.py` & `qs_codec-0.1.5/src/qs_codec/utils/str_utils.py`

 * *Files identical despite different names*

### Comparing `qs_codec-0.1.4/src/qs_codec/utils/utils.py` & `qs_codec-0.1.5/src/qs_codec/utils/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -188,20 +188,20 @@
                 if not Utils._dicts_are_equal(v, d2[k], path):
                     return False
             return True
         else:
             return d1 == d2
 
     @staticmethod
-    def combine(a: t.Union[t.Sequence, t.Any], b: t.Union[t.Sequence, t.Any]) -> t.List:
+    def combine(a: t.Union[list, tuple, t.Any], b: t.Union[list, tuple, t.Any]) -> t.List:
         """Combine two lists or values."""
         return [*(a if isinstance(a, (list, tuple)) else [a]), *(b if isinstance(b, (list, tuple)) else [b])]
 
     @staticmethod
-    def apply(val: t.Union[t.Sequence, t.Any], fn: t.Callable) -> t.Union[t.List, t.Any]:
+    def apply(val: t.Union[list, tuple, t.Any], fn: t.Callable) -> t.Union[t.List, t.Any]:
         """Apply a function to a value or a list of values."""
         return [fn(item) for item in val] if isinstance(val, (list, tuple)) else fn(val)
 
     @staticmethod
     def is_non_nullish_primitive(val: t.Any, skip_nulls: bool = False) -> bool:
         """Check if a value is a non-nullish primitive."""
         if val is None:
@@ -213,12 +213,12 @@
         if isinstance(val, (int, float, Decimal, bool, Enum, datetime, timedelta)):
             return True
 
         if isinstance(val, Undefined):
             return False
 
         if isinstance(val, object):
-            if isinstance(val, (t.Sequence, t.Mapping)):
+            if isinstance(val, (list, tuple, t.Mapping)):
                 return False
             return True
 
         return False
```

### Comparing `qs_codec-0.1.4/tests/comparison/qs.py` & `qs_codec-0.1.5/tests/comparison/qs.py`

 * *Files identical despite different names*

### Comparing `qs_codec-0.1.4/tests/comparison/test_cases.json` & `qs_codec-0.1.5/tests/comparison/test_cases.json`

 * *Files identical despite different names*

### Comparing `qs_codec-0.1.4/tests/e2e/e2e_test.py` & `qs_codec-0.1.5/tests/e2e/e2e_test.py`

 * *Files identical despite different names*

### Comparing `qs_codec-0.1.4/tests/unit/decode_test.py` & `qs_codec-0.1.5/tests/unit/decode_test.py`

 * *Files identical despite different names*

### Comparing `qs_codec-0.1.4/tests/unit/encode_test.py` & `qs_codec-0.1.5/tests/unit/encode_test.py`

 * *Files identical despite different names*

### Comparing `qs_codec-0.1.4/tests/unit/example_test.py` & `qs_codec-0.1.5/tests/unit/example_test.py`

 * *Files identical despite different names*

### Comparing `qs_codec-0.1.4/tests/unit/utils_test.py` & `qs_codec-0.1.5/tests/unit/utils_test.py`

 * *Files identical despite different names*

### Comparing `qs_codec-0.1.4/tests/unit/weakref_test.py` & `qs_codec-0.1.5/tests/unit/weakref_test.py`

 * *Files identical despite different names*

### Comparing `qs_codec-0.1.4/.gitignore` & `qs_codec-0.1.5/.gitignore`

 * *Files identical despite different names*

### Comparing `qs_codec-0.1.4/LICENSE` & `qs_codec-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `qs_codec-0.1.4/README.md` & `qs_codec-0.1.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 ) -> dict:
     """Decodes a str or Mapping into a Dict. 
     
     Providing custom DecodeOptions will override the default behavior."""
     pass
 ```
 
-**qs** allows you to create nested `dict`s within your query strings, by surrounding the name of sub-keys with 
+**qs_codec** allows you to create nested `dict`s within your query strings, by surrounding the name of sub-keys with 
 square brackets `[]`. For example, the string `'foo[bar]=baz'` converts to:
 
 ```python
 import qs_codec
 
 assert qs_codec.decode('foo[bar]=baz') == {'foo': {'bar': 'baz'}}
 ```
@@ -68,15 +68,15 @@
 ```python
 import qs_codec
 
 assert qs_codec.decode('foo[bar][baz]=foobarbaz') == {'foo': {'bar': {'baz': 'foobarbaz'}}}
 ```
 
 By default, when nesting `dict`s qs will only decode up to 5 children deep. This means if you attempt to decode a string 
-like 'a[b][c][d][e][f][g][h][i]=j' your resulting `dict` will be:
+like `'a[b][c][d][e][f][g][h][i]=j'` your resulting `dict` will be:
 
 ```python
 import qs_codec
 
 assert qs_codec.decode("a[b][c][d][e][f][g][h][i]=j") == {
     "a": {"b": {"c": {"d": {"e": {"f": {"[g][h][i]": "j"}}}}}}
 }
@@ -89,19 +89,19 @@
 
 assert qs_codec.decode(
     'a[b][c][d][e][f][g][h][i]=j',
     qs_codec.DecodeOptions(depth=1),
 ) == {'a': {'b': {'[c][d][e][f][g][h][i]': 'j'}}}
 ```
 
-The depth limit helps mitigate abuse when **qs** is used to parse user input, and it is recommended to keep it a
+The depth limit helps mitigate abuse when **qs_codec** is used to parse user input, and it is recommended to keep it a
 reasonably small number.
 
-For similar reasons, by default **qs** will only parse up to 1000 parameters. This can be overridden by passing 
-a `qs.DecodeOptions.parameter_limit` option:
+For similar reasons, by default **qs_codec** will only parse up to 1000 parameters. This can be overridden by passing 
+a `DecodeOptions.parameter_limit` option:
 
 ```python
 import qs_codec
 
 assert qs_codec.decode(
     'a=b&c=d',
     qs_codec.DecodeOptions(parameter_limit=1),
@@ -213,15 +213,15 @@
 ```
 
 Some services add an initial `utf8=✓` value to forms so that old Internet Explorer versions are more likely to submit the
 form as utf-8. Additionally, the server can check the value against wrong encodings of the checkmark character and detect 
 that a query string or `application/x-www-form-urlencoded` body was *not* sent as utf-8, eg. if the form had an 
 `accept-charset` parameter or the containing page had a different character set.
 
-**qs** supports this mechanism via the `DecodeOptions.charset_sentinel` option.
+**qs_codec** supports this mechanism via the `DecodeOptions.charset_sentinel` option.
 If specified, the `utf8` parameter will be omitted from the returned `dict`.
 It will be used to switch to `Charset.LATIN1`/`Charset.UTF8` mode depending on how the checkmark is encoded.
 
 **Important**: When you specify both the `DecodeOptions.charset` option and the `DecodeOptions.charset_sentinel` option, 
 the `DecodeOptions.charset` will be overridden when the request contains a `utf8` parameter from which the actual charset 
 can be deduced. In that sense the `DecodeOptions.charset` will behave as the default charset rather than the authoritative 
 charset.
@@ -261,15 +261,15 @@
 ) == {'a': '☺'}
 ```
 
 It also works when the charset has been detected in `DecodeOptions.charset_sentinel` mode.
 
 ### Decoding `list`s
 
-**qs** can also decode `list`s using a similar `[]` notation:
+**qs_codec** can also decode `list`s using a similar `[]` notation:
 
 ```python
 import qs_codec
 
 assert qs_codec.decode('a[]=b&a[]=c') == {'a': ['b', 'c']}
 ```
 
@@ -278,15 +278,15 @@
 ```python
 import qs_codec
 
 assert qs_codec.decode('a[1]=c&a[0]=b') == {'a': ['b', 'c']}
 ```
 
 Note that the only difference between an index in a `list` and a key in a `dict` is that the value between the brackets
-must be a number to create a `list`. When creating `list`s with specific indices, **qs** will compact a sparse 
+must be a number to create a `list`. When creating `list`s with specific indices, **qs_codec** will compact a sparse 
 `list` to only the existing values preserving their order:
 
 ```python
 import qs_codec
 
 assert qs_codec.decode('a[1]=b&a[15]=c') == {'a': ['b', 'c']}
 ```
@@ -297,15 +297,15 @@
 import qs_codec
 
 assert qs_codec.decode('a[]=&a[]=b') == {'a': ['', 'b']}
 
 assert qs_codec.decode('a[0]=b&a[1]=&a[2]=c') == {'a': ['b', '', 'c']}
 ```
 
-**qs** will also limit specifying indices in a `list` to a maximum index of `20`.
+**qs_codec** will also limit specifying indices in a `list` to a maximum index of `20`.
 Any `list` members with an index of greater than `20` will instead be converted to a `dict` with the index as the key.
 This is needed to handle cases when someone sent, for example, `a[999999999]` and it will take significant time to iterate 
 over this huge `list`.
 
 ```python
 import qs_codec
 
@@ -324,15 +324,15 @@
 
 ```python
 import qs_codec
 
 assert qs_codec.decode('a[]=b', qs_codec.DecodeOptions(parse_lists=False)) == {'a': {0: 'b'}}
 ```
 
-If you mix notations, **qs** will merge the two items into a `dict`:
+If you mix notations, **qs_codec** will merge the two items into a `dict`:
 
 ```python
 import qs_codec
 
 assert qs_codec.decode('a[0]=b&a[b]=c') == {'a': {0: 'b', 'b': 'c'}}
 ```
 
@@ -340,19 +340,19 @@
 
 ```python
 import qs_codec
 
 assert qs_codec.decode('a[][b]=c') == {'a': [{'b': 'c'}]}
 ```
 
-(_**qs** cannot convert nested `dict`s, such as `'a={b:1},{c:d}'`_)
+(_**qs_codec** cannot convert nested `dict`s, such as `'a={b:1},{c:d}'`_)
 
 ### Decoding primitive/scalar values (`int`, `float`, `bool`, `None`, etc.)
 
-By default, all values are parsed as `str`s.
+By default, all values are parsed as `str`ings.
 
 ```python
 import qs_codec
 
 assert qs_codec.decode('a=15&b=true&c=null') == {'a': '15', 'b': 'true', 'c': 'null'}
 ```
 
@@ -368,15 +368,15 @@
 ) -> str:
     """Encodes an object into a query string.
     
     Providing custom EncodeOptions will override the default behavior."""
     pass
 ```
 
-When encoding, **qs** by default URI encodes output. `dict`s are encoded as you would expect:
+When encoding, **qs_codec** by default URI encodes output. `dict`s are encoded as you would expect:
 
 ```python
 import qs_codec
 
 assert qs_codec.encode({'a': 'b'}) == 'a=b'
 assert qs_codec.encode({'a': {'b': 'c'}}) == 'a%5Bb%5D=c'
 ```
@@ -406,25 +406,25 @@
             ['h']
         ]
     },
     qs_codec.EncodeOptions(encode_values_only=True)
 ) == 'a=b&c[0]=d&c[1]=e%3Df&f[0][0]=g&f[1][0]=h'
 ```
 
-This encoding can also be replaced by a custom `Encoder` set as `EncodeOptions.encoder` option:
+This encoding can also be replaced by a custom `Callable` set in the `EncodeOptions.encoder` option:
 
 ```python
 import qs_codec, typing as t
 
 
 def custom_encoder(
-        value: str,
-        charset: t.Optional[qs_codec.Charset],
-        format: t.Optional[qs_codec.Format],
-):
+    value: str,
+    charset: t.Optional[qs_codec.Charset],
+    format: t.Optional[qs_codec.Format],
+) -> str:
     if value == 'č':
         return 'c'
     return value
 
 
 assert qs_codec.encode(
     {'a': {'b': 'č'}},
@@ -436,25 +436,23 @@
 
 Similar to `EncodeOptions.encoder` there is a `DecodeOptions.decoder` option for `decode` to override decoding of 
 properties and values:
 
 ```python
 import qs_codec, typing as t
 
-
 def custom_decoder(
-        value: t.Any,
-        charset: t.Optional[qs_codec.Charset],
-):
+    value: t.Any,
+    charset: t.Optional[qs_codec.Charset],
+) -> t.Union[int, str]:
     try:
         return int(value)
     except ValueError:
         return value
 
-
 assert qs_codec.decode(
     'foo=123',
     qs_codec.DecodeOptions(decoder=custom_decoder),
 ) == {'foo': 123}
 ```
 
 Examples beyond this point will be shown as though the output is not URI encoded for clarity.
@@ -468,15 +466,15 @@
 assert qs_codec.encode(
     {'a': ['b', 'c', 'd']},
     qs_codec.EncodeOptions(encode=False)
 ) == 'a[0]=b&a[1]=c&a[2]=d'
 ```
 
 You may override this by setting the `EncodeOptions.indices` option to `False`, or to be more explicit, the
-`EncodeOptions.list_lormat` option to `ListFormat.REPEAT`:
+`EncodeOptions.list_format` option to `ListFormat.REPEAT`:
 
 ```python
 import qs_codec
 
 assert qs_codec.encode(
     {'a': ['b', 'c', 'd']},
     qs_codec.EncodeOptions(
@@ -487,55 +485,55 @@
 ```
 
 You may use the `EncodeOptions.list_format` option to specify the format of the output `list`:
 
 ```python
 import qs_codec
 
-# For ListFormat.indices
+# ListFormat.INDICES
 assert qs_codec.encode(
     {'a': ['b', 'c']},
     qs_codec.EncodeOptions(
         encode=False,
         list_format=qs_codec.ListFormat.INDICES,
     ),
 ) == 'a[0]=b&a[1]=c'
 
-# For ListFormat.brackets
+# ListFormat.BRACKETS
 assert qs_codec.encode(
     {'a': ['b', 'c']},
     qs_codec.EncodeOptions(
         encode=False,
         list_format=qs_codec.ListFormat.BRACKETS,
     ),
 ) == 'a[]=b&a[]=c'
 
-# For ListFormat.repeat
+# ListFormat.REPEAT
 assert qs_codec.encode(
     {'a': ['b', 'c']},
     qs_codec.EncodeOptions(
         encode=False,
         list_format=qs_codec.ListFormat.REPEAT,
     ),
 ) == 'a=b&a=c'
 
-# For ListFormat.comma
+# ListFormat.COMMA
 assert qs_codec.encode(
     {'a': ['b', 'c']},
     qs_codec.EncodeOptions(
         encode=False,
         list_format=qs_codec.ListFormat.COMMA,
     ),
 ) == 'a=b,c'
 ```
 
 **Note:** When using `EncodeOptions.list_format` set to `ListFormat.COMMA`, you can also pass the `EncodeOptions.comma_round_trip`
 option set to `True` or `False`, to append `[]` on single-item `list`s, so that they can round trip through a parse.
 
-When `dict`s are encoded, by default they use bracket notation:
+`ListFormat.BRACKETS` notation is used for encoding `dict`s by default:
 
 ```python
 import qs_codec
 
 assert qs_codec.encode(
     {'a': {'b': {'c': 'd', 'e': 'f'}}},
     qs_codec.EncodeOptions(encode=False),
@@ -549,30 +547,30 @@
 
 assert qs_codec.encode(
     {'a': {'b': {'c': 'd', 'e': 'f'}}},
     qs_codec.EncodeOptions(encode=False, allow_dots=True),
 ) == 'a.b.c=d&a.b.e=f'
 ```
 
-You may encode the dot notation in the keys of `dict` with option `EncodeOptions.encode_dot_in_keys` by setting it to `True`:
+You may encode dots in keys of `dict`s by setting `EncodeOptions.encode_dot_in_keys` to `True`:
 
 ```python
 import qs_codec
 
 assert qs_codec.encode(
     {'name.obj': {'first': 'John', 'last': 'Doe'}},
     qs_codec.EncodeOptions(
         allow_dots=True,
         encode_dot_in_keys=True,
     ),
 ) == 'name%252Eobj.first=John&name%252Eobj.last=Doe'
 ```
 
-**Caveat:** when `EncodeOptions.encode_values_only` is `True` as well as `EncodeOptions.encode_dot_in_keys`, only dots in 
-keys and nothing else will be encoded.
+**Caveat:** When both `EncodeOptions.encode_values_only` and `EncodeOptions.encode_dot_in_keys` are set to `True`, only
+dots in keys and nothing else will be encoded!
 
 You may allow empty `list` values by setting the `EncodeOptions.allow_empty_lists` option to `True`:
 
 ```python
 import qs_codec
 
 assert qs_codec.encode(
@@ -580,23 +578,23 @@
     qs_codec.EncodeOptions(
         encode=False,
         allow_empty_lists=True,
     ),
 ) == 'foo[]&bar=baz'
 ```
 
-Empty strings and null values will omit the value, but the equals sign (`=`) remains in place:
+Empty `str`ings and `None` values will be omitted, but the equals sign (`=`) remains in place:
 
 ```python
 import qs_codec
 
 assert qs_codec.encode({'a': ''}) == 'a='
 ```
 
-Key with no values (such as an empty `dict` or `list`) will return nothing:
+Keys with no values (such as an empty `dict` or `list`) will return nothing:
 
 ```python
 import qs_codec
 
 assert qs_codec.encode({'a': []}) == ''
 
 assert qs_codec.encode({'a': {}}) == ''
@@ -604,23 +602,23 @@
 assert qs_codec.encode({'a': [{}]}) == ''
 
 assert qs_codec.encode({'a': {'b': []}}) == ''
 
 assert qs_codec.encode({'a': {'b': {}}}) == ''
 ```
 
-Properties that are `Undefined` will be omitted entirely:
+`Undefined` properties will be omitted entirely:
 
 ```python
 import qs_codec
 
 assert qs_codec.encode({'a': None, 'b': qs_codec.Undefined()}) == 'a='
 ```
 
-The query string may optionally be prepended with a question mark:
+The query string may optionally be prepended with a question mark (`?`):
 
 ```python
 import qs_codec
 
 assert qs_codec.encode(
     {'a': 'b', 'c': 'd'},
     qs_codec.EncodeOptions(add_query_prefix=True),
@@ -634,15 +632,15 @@
 
 assert qs_codec.encode(
     {'a': 'b', 'c': 'd', },
     qs_codec.EncodeOptions(delimiter=';')
 ) == 'a=b;c=d'
 ```
 
-If you only want to override the serialization of `datetime.datetime` objects, you can provide a custom `DateSerializer`
+If you only want to override the serialization of `datetime` objects, you can provide a custom `DateSerializer`
 in the `EncodeOptions.serialize_date` option:
 
 ```python
 import qs_codec, datetime, sys
 
 # First case: encoding a datetime object to an ISO 8601 string
 assert (
@@ -659,29 +657,29 @@
     == "a=1970-01-01T00:00:07+00:00"
     if sys.version_info.major == 3 and sys.version_info.minor >= 11
     else "a=1970-01-01T00:00:07"
 )
 
 # Second case: encoding a datetime object to a timestamp string
 assert (
-        qs_codec.encode(
-            {
-                "a": (
-                    datetime.datetime.fromtimestamp(7, datetime.UTC)
-                    if sys.version_info.major == 3 and sys.version_info.minor >= 11
-                    else datetime.datetime.utcfromtimestamp(7)
-                )
-            },
-            qs_codec.EncodeOptions(encode=False, serialize_date=lambda date: str(int(date.timestamp()))),
-        )
-        == "a=7"
+    qs_codec.encode(
+        {
+            "a": (
+                datetime.datetime.fromtimestamp(7, datetime.UTC)
+                if sys.version_info.major == 3 and sys.version_info.minor >= 11
+                else datetime.datetime.utcfromtimestamp(7)
+            )
+        },
+        qs_codec.EncodeOptions(encode=False, serialize_date=lambda date: str(int(date.timestamp()))),
+    )
+    == "a=7"
 )
 ```
 
-You may use the `EncodeOptions.sort` option to affect the order of parameter keys:
+To affect the order of parameter keys, you can set a `Callable` in the `EncodeOptions.sort` option:
 
 ```python
 import qs_codec
 
 assert qs_codec.encode(
     {'a': 'c', 'z': 'y', 'b': 'f'},
     qs_codec.EncodeOptions(
@@ -694,39 +692,39 @@
 Finally, you can use the `EncodeOptions.filter` option to restrict which keys will be included in the encoded output.
 If you pass a `Callable`, it will be called for each key to obtain the replacement value.
 Otherwise, if you pass a `list`, it will be used to select properties and `list` indices to be encoded:
 
 ```python
 import qs_codec, datetime, sys
 
-# First case: using a function as filter
+# First case: using a Callable as filter
 assert (
-        qs_codec.encode(
-            {
-                "a": "b",
-                "c": "d",
-                "e": {
-                    "f": (
-                        datetime.datetime.fromtimestamp(123, datetime.UTC)
-                        if sys.version_info.major == 3 and sys.version_info.minor >= 11
-                        else datetime.datetime.utcfromtimestamp(123)
-                    ),
-                    "g": [2],
-                },
+    qs_codec.encode(
+        {
+            "a": "b",
+            "c": "d",
+            "e": {
+                "f": (
+                    datetime.datetime.fromtimestamp(123, datetime.UTC)
+                    if sys.version_info.major == 3 and sys.version_info.minor >= 11
+                    else datetime.datetime.utcfromtimestamp(123)
+                ),
+                "g": [2],
             },
-            qs_codec.EncodeOptions(
-                encode=False,
-                filter=lambda prefix, value: {
-                    "b": None,
-                    "e[f]": int(value.timestamp()) if isinstance(value, datetime.datetime) else value,
-                    "e[g][0]": value * 2 if isinstance(value, int) else value,
-                }.get(prefix, value),
-            ),
-        )
-        == "a=b&c=d&e[f]=123&e[g][0]=4"
+        },
+        qs_codec.EncodeOptions(
+            encode=False,
+            filter=lambda prefix, value: {
+                "b": None,
+                "e[f]": int(value.timestamp()) if isinstance(value, datetime.datetime) else value,
+                "e[g][0]": value * 2 if isinstance(value, int) else value,
+            }.get(prefix, value),
+        ),
+    )
+    == "a=b&c=d&e[f]=123&e[g][0]=4"
 )
 
 # Second case: using a list as filter
 assert qs_codec.encode(
     {'a': 'b', 'c': 'd', 'e': 'f'},
     qs_codec.EncodeOptions(
         encode=False,
@@ -743,17 +741,17 @@
     qs_codec.EncodeOptions(
         encode=False,
         filter=['a', 0, 2]
     )
 ) == 'a[0]=b&a[2]=d'
 ```
 
-### Handling of `None` values
+### Handling `None` values
 
-By default, `None` values are treated like empty strings:
+By default, `None` values are treated like empty `str`ings:
 
 ```python
 import qs_codec
 
 assert qs_codec.encode({'a': None, 'b': ''}) == 'a=&b='
 ```
 
@@ -839,55 +837,53 @@
 [Shift JIS](https://en.wikipedia.org/wiki/Shift_JIS))
 
 ```python
 import qs_codec, codecs, typing as t
 
 
 def custom_encoder(
-        string: str,
-        charset: t.Optional[qs_codec.Charset],
-        format: t.Optional[qs_codec.Format],
+    string: str,
+    charset: t.Optional[qs_codec.Charset],
+    format: t.Optional[qs_codec.Format],
 ) -> str:
     if string:
         buf: bytes = codecs.encode(string, 'shift_jis')
         result: t.List[str] = ['{:02x}'.format(b) for b in buf]
         return '%' + '%'.join(result)
     return ''
 
-
 assert qs_codec.encode(
     {'a': 'こんにちは！'},
     qs_codec.EncodeOptions(encoder=custom_encoder)
 ) == '%61=%82%b1%82%f1%82%c9%82%bf%82%cd%81%49'
 ```
 
 This also works for decoding of query strings:
 
 ```python
 import qs_codec, re, codecs, typing as t
 
 
 def custom_decoder(
-        string: str,
-        charset: t.Optional[qs_codec.Charset],
+    string: str,
+    charset: t.Optional[qs_codec.Charset],
 ) -> t.Optional[str]:
     if string:
         result: t.List[int] = []
         while string:
             match: t.Optional[t.Match[str]] = re.search(r'%([0-9A-F]{2})', string, re.IGNORECASE)
             if match:
                 result.append(int(match.group(1), 16))
                 string = string[match.end():]
             else:
                 break
         buf: bytes = bytes(result)
         return codecs.decode(buf, 'shift_jis')
     return None
 
-
 assert qs_codec.decode(
     '%61=%82%b1%82%f1%82%c9%82%bf%82%cd%81%49',
     qs_codec.DecodeOptions(decoder=custom_decoder)
 ) == {'a': 'こんにちは！'}
 ```
 
 ### RFC 3986 and RFC 1738 space encoding
```

### Comparing `qs_codec-0.1.4/pyproject.toml` & `qs_codec-0.1.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 description = "A query string encoding and decoding library for Python. Ported from qs for JavaScript."
 readme = "README.md"
 license = { text = "BSD-3-Clause" }
 requires-python = ">=3.8"
 authors = [
     { name = "Klemen Tusar", email = "techouse@gmail.com" },
 ]
+documentation = "https://techouse.github.io/qs_codec/"
 keywords = [
     "qs",
     "codec",
     "url",
     "query",
     "querystring",
     "query-string",
```

### Comparing `qs_codec-0.1.4/PKG-INFO` & `qs_codec-0.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: qs-codec
-Version: 0.1.4
+Version: 0.1.5
 Summary: A query string encoding and decoding library for Python. Ported from qs for JavaScript.
 Project-URL: Source, https://github.com/techouse/qs_codec
 Project-URL: Changelog, https://github.com/techouse/qs_codec/blob/master/CHANGELOG.md
 Project-URL: Sponsor, https://github.com/sponsors/techouse
 Project-URL: PayPal, https://paypal.me/ktusar
 Author-email: Klemen Tusar <techouse@gmail.com>
 License: BSD-3-Clause
@@ -75,15 +75,15 @@
 ) -> dict:
     """Decodes a str or Mapping into a Dict. 
     
     Providing custom DecodeOptions will override the default behavior."""
     pass
 ```
 
-**qs** allows you to create nested `dict`s within your query strings, by surrounding the name of sub-keys with 
+**qs_codec** allows you to create nested `dict`s within your query strings, by surrounding the name of sub-keys with 
 square brackets `[]`. For example, the string `'foo[bar]=baz'` converts to:
 
 ```python
 import qs_codec
 
 assert qs_codec.decode('foo[bar]=baz') == {'foo': {'bar': 'baz'}}
 ```
@@ -101,15 +101,15 @@
 ```python
 import qs_codec
 
 assert qs_codec.decode('foo[bar][baz]=foobarbaz') == {'foo': {'bar': {'baz': 'foobarbaz'}}}
 ```
 
 By default, when nesting `dict`s qs will only decode up to 5 children deep. This means if you attempt to decode a string 
-like 'a[b][c][d][e][f][g][h][i]=j' your resulting `dict` will be:
+like `'a[b][c][d][e][f][g][h][i]=j'` your resulting `dict` will be:
 
 ```python
 import qs_codec
 
 assert qs_codec.decode("a[b][c][d][e][f][g][h][i]=j") == {
     "a": {"b": {"c": {"d": {"e": {"f": {"[g][h][i]": "j"}}}}}}
 }
@@ -122,19 +122,19 @@
 
 assert qs_codec.decode(
     'a[b][c][d][e][f][g][h][i]=j',
     qs_codec.DecodeOptions(depth=1),
 ) == {'a': {'b': {'[c][d][e][f][g][h][i]': 'j'}}}
 ```
 
-The depth limit helps mitigate abuse when **qs** is used to parse user input, and it is recommended to keep it a
+The depth limit helps mitigate abuse when **qs_codec** is used to parse user input, and it is recommended to keep it a
 reasonably small number.
 
-For similar reasons, by default **qs** will only parse up to 1000 parameters. This can be overridden by passing 
-a `qs.DecodeOptions.parameter_limit` option:
+For similar reasons, by default **qs_codec** will only parse up to 1000 parameters. This can be overridden by passing 
+a `DecodeOptions.parameter_limit` option:
 
 ```python
 import qs_codec
 
 assert qs_codec.decode(
     'a=b&c=d',
     qs_codec.DecodeOptions(parameter_limit=1),
@@ -246,15 +246,15 @@
 ```
 
 Some services add an initial `utf8=✓` value to forms so that old Internet Explorer versions are more likely to submit the
 form as utf-8. Additionally, the server can check the value against wrong encodings of the checkmark character and detect 
 that a query string or `application/x-www-form-urlencoded` body was *not* sent as utf-8, eg. if the form had an 
 `accept-charset` parameter or the containing page had a different character set.
 
-**qs** supports this mechanism via the `DecodeOptions.charset_sentinel` option.
+**qs_codec** supports this mechanism via the `DecodeOptions.charset_sentinel` option.
 If specified, the `utf8` parameter will be omitted from the returned `dict`.
 It will be used to switch to `Charset.LATIN1`/`Charset.UTF8` mode depending on how the checkmark is encoded.
 
 **Important**: When you specify both the `DecodeOptions.charset` option and the `DecodeOptions.charset_sentinel` option, 
 the `DecodeOptions.charset` will be overridden when the request contains a `utf8` parameter from which the actual charset 
 can be deduced. In that sense the `DecodeOptions.charset` will behave as the default charset rather than the authoritative 
 charset.
@@ -294,15 +294,15 @@
 ) == {'a': '☺'}
 ```
 
 It also works when the charset has been detected in `DecodeOptions.charset_sentinel` mode.
 
 ### Decoding `list`s
 
-**qs** can also decode `list`s using a similar `[]` notation:
+**qs_codec** can also decode `list`s using a similar `[]` notation:
 
 ```python
 import qs_codec
 
 assert qs_codec.decode('a[]=b&a[]=c') == {'a': ['b', 'c']}
 ```
 
@@ -311,15 +311,15 @@
 ```python
 import qs_codec
 
 assert qs_codec.decode('a[1]=c&a[0]=b') == {'a': ['b', 'c']}
 ```
 
 Note that the only difference between an index in a `list` and a key in a `dict` is that the value between the brackets
-must be a number to create a `list`. When creating `list`s with specific indices, **qs** will compact a sparse 
+must be a number to create a `list`. When creating `list`s with specific indices, **qs_codec** will compact a sparse 
 `list` to only the existing values preserving their order:
 
 ```python
 import qs_codec
 
 assert qs_codec.decode('a[1]=b&a[15]=c') == {'a': ['b', 'c']}
 ```
@@ -330,15 +330,15 @@
 import qs_codec
 
 assert qs_codec.decode('a[]=&a[]=b') == {'a': ['', 'b']}
 
 assert qs_codec.decode('a[0]=b&a[1]=&a[2]=c') == {'a': ['b', '', 'c']}
 ```
 
-**qs** will also limit specifying indices in a `list` to a maximum index of `20`.
+**qs_codec** will also limit specifying indices in a `list` to a maximum index of `20`.
 Any `list` members with an index of greater than `20` will instead be converted to a `dict` with the index as the key.
 This is needed to handle cases when someone sent, for example, `a[999999999]` and it will take significant time to iterate 
 over this huge `list`.
 
 ```python
 import qs_codec
 
@@ -357,15 +357,15 @@
 
 ```python
 import qs_codec
 
 assert qs_codec.decode('a[]=b', qs_codec.DecodeOptions(parse_lists=False)) == {'a': {0: 'b'}}
 ```
 
-If you mix notations, **qs** will merge the two items into a `dict`:
+If you mix notations, **qs_codec** will merge the two items into a `dict`:
 
 ```python
 import qs_codec
 
 assert qs_codec.decode('a[0]=b&a[b]=c') == {'a': {0: 'b', 'b': 'c'}}
 ```
 
@@ -373,19 +373,19 @@
 
 ```python
 import qs_codec
 
 assert qs_codec.decode('a[][b]=c') == {'a': [{'b': 'c'}]}
 ```
 
-(_**qs** cannot convert nested `dict`s, such as `'a={b:1},{c:d}'`_)
+(_**qs_codec** cannot convert nested `dict`s, such as `'a={b:1},{c:d}'`_)
 
 ### Decoding primitive/scalar values (`int`, `float`, `bool`, `None`, etc.)
 
-By default, all values are parsed as `str`s.
+By default, all values are parsed as `str`ings.
 
 ```python
 import qs_codec
 
 assert qs_codec.decode('a=15&b=true&c=null') == {'a': '15', 'b': 'true', 'c': 'null'}
 ```
 
@@ -401,15 +401,15 @@
 ) -> str:
     """Encodes an object into a query string.
     
     Providing custom EncodeOptions will override the default behavior."""
     pass
 ```
 
-When encoding, **qs** by default URI encodes output. `dict`s are encoded as you would expect:
+When encoding, **qs_codec** by default URI encodes output. `dict`s are encoded as you would expect:
 
 ```python
 import qs_codec
 
 assert qs_codec.encode({'a': 'b'}) == 'a=b'
 assert qs_codec.encode({'a': {'b': 'c'}}) == 'a%5Bb%5D=c'
 ```
@@ -439,25 +439,25 @@
             ['h']
         ]
     },
     qs_codec.EncodeOptions(encode_values_only=True)
 ) == 'a=b&c[0]=d&c[1]=e%3Df&f[0][0]=g&f[1][0]=h'
 ```
 
-This encoding can also be replaced by a custom `Encoder` set as `EncodeOptions.encoder` option:
+This encoding can also be replaced by a custom `Callable` set in the `EncodeOptions.encoder` option:
 
 ```python
 import qs_codec, typing as t
 
 
 def custom_encoder(
-        value: str,
-        charset: t.Optional[qs_codec.Charset],
-        format: t.Optional[qs_codec.Format],
-):
+    value: str,
+    charset: t.Optional[qs_codec.Charset],
+    format: t.Optional[qs_codec.Format],
+) -> str:
     if value == 'č':
         return 'c'
     return value
 
 
 assert qs_codec.encode(
     {'a': {'b': 'č'}},
@@ -469,25 +469,23 @@
 
 Similar to `EncodeOptions.encoder` there is a `DecodeOptions.decoder` option for `decode` to override decoding of 
 properties and values:
 
 ```python
 import qs_codec, typing as t
 
-
 def custom_decoder(
-        value: t.Any,
-        charset: t.Optional[qs_codec.Charset],
-):
+    value: t.Any,
+    charset: t.Optional[qs_codec.Charset],
+) -> t.Union[int, str]:
     try:
         return int(value)
     except ValueError:
         return value
 
-
 assert qs_codec.decode(
     'foo=123',
     qs_codec.DecodeOptions(decoder=custom_decoder),
 ) == {'foo': 123}
 ```
 
 Examples beyond this point will be shown as though the output is not URI encoded for clarity.
@@ -501,15 +499,15 @@
 assert qs_codec.encode(
     {'a': ['b', 'c', 'd']},
     qs_codec.EncodeOptions(encode=False)
 ) == 'a[0]=b&a[1]=c&a[2]=d'
 ```
 
 You may override this by setting the `EncodeOptions.indices` option to `False`, or to be more explicit, the
-`EncodeOptions.list_lormat` option to `ListFormat.REPEAT`:
+`EncodeOptions.list_format` option to `ListFormat.REPEAT`:
 
 ```python
 import qs_codec
 
 assert qs_codec.encode(
     {'a': ['b', 'c', 'd']},
     qs_codec.EncodeOptions(
@@ -520,55 +518,55 @@
 ```
 
 You may use the `EncodeOptions.list_format` option to specify the format of the output `list`:
 
 ```python
 import qs_codec
 
-# For ListFormat.indices
+# ListFormat.INDICES
 assert qs_codec.encode(
     {'a': ['b', 'c']},
     qs_codec.EncodeOptions(
         encode=False,
         list_format=qs_codec.ListFormat.INDICES,
     ),
 ) == 'a[0]=b&a[1]=c'
 
-# For ListFormat.brackets
+# ListFormat.BRACKETS
 assert qs_codec.encode(
     {'a': ['b', 'c']},
     qs_codec.EncodeOptions(
         encode=False,
         list_format=qs_codec.ListFormat.BRACKETS,
     ),
 ) == 'a[]=b&a[]=c'
 
-# For ListFormat.repeat
+# ListFormat.REPEAT
 assert qs_codec.encode(
     {'a': ['b', 'c']},
     qs_codec.EncodeOptions(
         encode=False,
         list_format=qs_codec.ListFormat.REPEAT,
     ),
 ) == 'a=b&a=c'
 
-# For ListFormat.comma
+# ListFormat.COMMA
 assert qs_codec.encode(
     {'a': ['b', 'c']},
     qs_codec.EncodeOptions(
         encode=False,
         list_format=qs_codec.ListFormat.COMMA,
     ),
 ) == 'a=b,c'
 ```
 
 **Note:** When using `EncodeOptions.list_format` set to `ListFormat.COMMA`, you can also pass the `EncodeOptions.comma_round_trip`
 option set to `True` or `False`, to append `[]` on single-item `list`s, so that they can round trip through a parse.
 
-When `dict`s are encoded, by default they use bracket notation:
+`ListFormat.BRACKETS` notation is used for encoding `dict`s by default:
 
 ```python
 import qs_codec
 
 assert qs_codec.encode(
     {'a': {'b': {'c': 'd', 'e': 'f'}}},
     qs_codec.EncodeOptions(encode=False),
@@ -582,30 +580,30 @@
 
 assert qs_codec.encode(
     {'a': {'b': {'c': 'd', 'e': 'f'}}},
     qs_codec.EncodeOptions(encode=False, allow_dots=True),
 ) == 'a.b.c=d&a.b.e=f'
 ```
 
-You may encode the dot notation in the keys of `dict` with option `EncodeOptions.encode_dot_in_keys` by setting it to `True`:
+You may encode dots in keys of `dict`s by setting `EncodeOptions.encode_dot_in_keys` to `True`:
 
 ```python
 import qs_codec
 
 assert qs_codec.encode(
     {'name.obj': {'first': 'John', 'last': 'Doe'}},
     qs_codec.EncodeOptions(
         allow_dots=True,
         encode_dot_in_keys=True,
     ),
 ) == 'name%252Eobj.first=John&name%252Eobj.last=Doe'
 ```
 
-**Caveat:** when `EncodeOptions.encode_values_only` is `True` as well as `EncodeOptions.encode_dot_in_keys`, only dots in 
-keys and nothing else will be encoded.
+**Caveat:** When both `EncodeOptions.encode_values_only` and `EncodeOptions.encode_dot_in_keys` are set to `True`, only
+dots in keys and nothing else will be encoded!
 
 You may allow empty `list` values by setting the `EncodeOptions.allow_empty_lists` option to `True`:
 
 ```python
 import qs_codec
 
 assert qs_codec.encode(
@@ -613,23 +611,23 @@
     qs_codec.EncodeOptions(
         encode=False,
         allow_empty_lists=True,
     ),
 ) == 'foo[]&bar=baz'
 ```
 
-Empty strings and null values will omit the value, but the equals sign (`=`) remains in place:
+Empty `str`ings and `None` values will be omitted, but the equals sign (`=`) remains in place:
 
 ```python
 import qs_codec
 
 assert qs_codec.encode({'a': ''}) == 'a='
 ```
 
-Key with no values (such as an empty `dict` or `list`) will return nothing:
+Keys with no values (such as an empty `dict` or `list`) will return nothing:
 
 ```python
 import qs_codec
 
 assert qs_codec.encode({'a': []}) == ''
 
 assert qs_codec.encode({'a': {}}) == ''
@@ -637,23 +635,23 @@
 assert qs_codec.encode({'a': [{}]}) == ''
 
 assert qs_codec.encode({'a': {'b': []}}) == ''
 
 assert qs_codec.encode({'a': {'b': {}}}) == ''
 ```
 
-Properties that are `Undefined` will be omitted entirely:
+`Undefined` properties will be omitted entirely:
 
 ```python
 import qs_codec
 
 assert qs_codec.encode({'a': None, 'b': qs_codec.Undefined()}) == 'a='
 ```
 
-The query string may optionally be prepended with a question mark:
+The query string may optionally be prepended with a question mark (`?`):
 
 ```python
 import qs_codec
 
 assert qs_codec.encode(
     {'a': 'b', 'c': 'd'},
     qs_codec.EncodeOptions(add_query_prefix=True),
@@ -667,15 +665,15 @@
 
 assert qs_codec.encode(
     {'a': 'b', 'c': 'd', },
     qs_codec.EncodeOptions(delimiter=';')
 ) == 'a=b;c=d'
 ```
 
-If you only want to override the serialization of `datetime.datetime` objects, you can provide a custom `DateSerializer`
+If you only want to override the serialization of `datetime` objects, you can provide a custom `DateSerializer`
 in the `EncodeOptions.serialize_date` option:
 
 ```python
 import qs_codec, datetime, sys
 
 # First case: encoding a datetime object to an ISO 8601 string
 assert (
@@ -692,29 +690,29 @@
     == "a=1970-01-01T00:00:07+00:00"
     if sys.version_info.major == 3 and sys.version_info.minor >= 11
     else "a=1970-01-01T00:00:07"
 )
 
 # Second case: encoding a datetime object to a timestamp string
 assert (
-        qs_codec.encode(
-            {
-                "a": (
-                    datetime.datetime.fromtimestamp(7, datetime.UTC)
-                    if sys.version_info.major == 3 and sys.version_info.minor >= 11
-                    else datetime.datetime.utcfromtimestamp(7)
-                )
-            },
-            qs_codec.EncodeOptions(encode=False, serialize_date=lambda date: str(int(date.timestamp()))),
-        )
-        == "a=7"
+    qs_codec.encode(
+        {
+            "a": (
+                datetime.datetime.fromtimestamp(7, datetime.UTC)
+                if sys.version_info.major == 3 and sys.version_info.minor >= 11
+                else datetime.datetime.utcfromtimestamp(7)
+            )
+        },
+        qs_codec.EncodeOptions(encode=False, serialize_date=lambda date: str(int(date.timestamp()))),
+    )
+    == "a=7"
 )
 ```
 
-You may use the `EncodeOptions.sort` option to affect the order of parameter keys:
+To affect the order of parameter keys, you can set a `Callable` in the `EncodeOptions.sort` option:
 
 ```python
 import qs_codec
 
 assert qs_codec.encode(
     {'a': 'c', 'z': 'y', 'b': 'f'},
     qs_codec.EncodeOptions(
@@ -727,39 +725,39 @@
 Finally, you can use the `EncodeOptions.filter` option to restrict which keys will be included in the encoded output.
 If you pass a `Callable`, it will be called for each key to obtain the replacement value.
 Otherwise, if you pass a `list`, it will be used to select properties and `list` indices to be encoded:
 
 ```python
 import qs_codec, datetime, sys
 
-# First case: using a function as filter
+# First case: using a Callable as filter
 assert (
-        qs_codec.encode(
-            {
-                "a": "b",
-                "c": "d",
-                "e": {
-                    "f": (
-                        datetime.datetime.fromtimestamp(123, datetime.UTC)
-                        if sys.version_info.major == 3 and sys.version_info.minor >= 11
-                        else datetime.datetime.utcfromtimestamp(123)
-                    ),
-                    "g": [2],
-                },
+    qs_codec.encode(
+        {
+            "a": "b",
+            "c": "d",
+            "e": {
+                "f": (
+                    datetime.datetime.fromtimestamp(123, datetime.UTC)
+                    if sys.version_info.major == 3 and sys.version_info.minor >= 11
+                    else datetime.datetime.utcfromtimestamp(123)
+                ),
+                "g": [2],
             },
-            qs_codec.EncodeOptions(
-                encode=False,
-                filter=lambda prefix, value: {
-                    "b": None,
-                    "e[f]": int(value.timestamp()) if isinstance(value, datetime.datetime) else value,
-                    "e[g][0]": value * 2 if isinstance(value, int) else value,
-                }.get(prefix, value),
-            ),
-        )
-        == "a=b&c=d&e[f]=123&e[g][0]=4"
+        },
+        qs_codec.EncodeOptions(
+            encode=False,
+            filter=lambda prefix, value: {
+                "b": None,
+                "e[f]": int(value.timestamp()) if isinstance(value, datetime.datetime) else value,
+                "e[g][0]": value * 2 if isinstance(value, int) else value,
+            }.get(prefix, value),
+        ),
+    )
+    == "a=b&c=d&e[f]=123&e[g][0]=4"
 )
 
 # Second case: using a list as filter
 assert qs_codec.encode(
     {'a': 'b', 'c': 'd', 'e': 'f'},
     qs_codec.EncodeOptions(
         encode=False,
@@ -776,17 +774,17 @@
     qs_codec.EncodeOptions(
         encode=False,
         filter=['a', 0, 2]
     )
 ) == 'a[0]=b&a[2]=d'
 ```
 
-### Handling of `None` values
+### Handling `None` values
 
-By default, `None` values are treated like empty strings:
+By default, `None` values are treated like empty `str`ings:
 
 ```python
 import qs_codec
 
 assert qs_codec.encode({'a': None, 'b': ''}) == 'a=&b='
 ```
 
@@ -872,55 +870,53 @@
 [Shift JIS](https://en.wikipedia.org/wiki/Shift_JIS))
 
 ```python
 import qs_codec, codecs, typing as t
 
 
 def custom_encoder(
-        string: str,
-        charset: t.Optional[qs_codec.Charset],
-        format: t.Optional[qs_codec.Format],
+    string: str,
+    charset: t.Optional[qs_codec.Charset],
+    format: t.Optional[qs_codec.Format],
 ) -> str:
     if string:
         buf: bytes = codecs.encode(string, 'shift_jis')
         result: t.List[str] = ['{:02x}'.format(b) for b in buf]
         return '%' + '%'.join(result)
     return ''
 
-
 assert qs_codec.encode(
     {'a': 'こんにちは！'},
     qs_codec.EncodeOptions(encoder=custom_encoder)
 ) == '%61=%82%b1%82%f1%82%c9%82%bf%82%cd%81%49'
 ```
 
 This also works for decoding of query strings:
 
 ```python
 import qs_codec, re, codecs, typing as t
 
 
 def custom_decoder(
-        string: str,
-        charset: t.Optional[qs_codec.Charset],
+    string: str,
+    charset: t.Optional[qs_codec.Charset],
 ) -> t.Optional[str]:
     if string:
         result: t.List[int] = []
         while string:
             match: t.Optional[t.Match[str]] = re.search(r'%([0-9A-F]{2})', string, re.IGNORECASE)
             if match:
                 result.append(int(match.group(1), 16))
                 string = string[match.end():]
             else:
                 break
         buf: bytes = bytes(result)
         return codecs.decode(buf, 'shift_jis')
     return None
 
-
 assert qs_codec.decode(
     '%61=%82%b1%82%f1%82%c9%82%bf%82%cd%81%49',
     qs_codec.DecodeOptions(decoder=custom_decoder)
 ) == {'a': 'こんにちは！'}
 ```
 
 ### RFC 3986 and RFC 1738 space encoding
```

