# Comparing `tmp/html_elements-0.1.4.tar.gz` & `tmp/html_elements-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "html_elements-0.1.4.tar", max compression
+gzip compressed data, was "html_elements-0.2.0.tar", max compression
```

## Comparing `html_elements-0.1.4.tar` & `html_elements-0.2.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1076 2024-03-22 09:26:50.620238 html_elements-0.1.4/LICENSE
--rw-r--r--   0        0        0     1555 2024-03-22 09:23:20.750337 html_elements-0.1.4/README.md
--rw-r--r--   0        0        0        0 2024-02-14 14:26:35.458394 html_elements-0.1.4/html_elements/__init__.py
--rw-r--r--   0        0        0    10919 2024-04-04 18:09:24.639187 html_elements-0.1.4/html_elements/base.py
--rw-r--r--   0        0        0    34848 2024-04-04 18:09:24.887636 html_elements-0.1.4/html_elements/elements.py
--rw-r--r--   0        0        0     4159 2024-03-01 08:37:04.759557 html_elements-0.1.4/html_elements/extensions.py
--rw-r--r--   0        0        0        0 2024-04-03 17:56:10.211171 html_elements-0.1.4/html_elements/py.typed
--rw-r--r--   0        0        0      941 2024-04-03 18:14:46.135024 html_elements-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     2185 1970-01-01 00:00:00.000000 html_elements-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1076 2024-03-22 09:26:50.620238 html_elements-0.2.0/LICENSE
+-rw-r--r--   0        0        0     1555 2024-03-22 09:23:20.750337 html_elements-0.2.0/README.md
+-rw-r--r--   0        0        0        0 2024-02-14 14:26:35.458394 html_elements-0.2.0/html_elements/__init__.py
+-rw-r--r--   0        0        0    11310 2024-04-29 18:00:53.216948 html_elements-0.2.0/html_elements/base.py
+-rw-r--r--   0        0        0    34848 2024-04-04 18:09:24.887636 html_elements-0.2.0/html_elements/elements.py
+-rw-r--r--   0        0        0     4159 2024-03-01 08:37:04.759557 html_elements-0.2.0/html_elements/extensions.py
+-rw-r--r--   0        0        0        0 2024-04-03 17:56:10.211171 html_elements-0.2.0/html_elements/py.typed
+-rw-r--r--   0        0        0      941 2024-04-29 18:02:19.722588 html_elements-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     2185 1970-01-01 00:00:00.000000 html_elements-0.2.0/PKG-INFO
```

### Comparing `html_elements-0.1.4/LICENSE` & `html_elements-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `html_elements-0.1.4/README.md` & `html_elements-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `html_elements-0.1.4/html_elements/base.py` & `html_elements-0.2.0/html_elements/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,11 @@
+import html
 from abc import ABC, ABCMeta
-from typing import TYPE_CHECKING, Any, Callable, ClassVar, Dict, List, Literal, Tuple, Type, TypedDict, Union
+from typing import (TYPE_CHECKING, Any, Callable, ClassVar, Dict, List,
+                    Literal, Tuple, Type, TypedDict, Union)
 
 from typing_extensions import dataclass_transform
 
 Undefined = object()
 HtmlAttributeType = Literal["attribute", "content"]
 
 
@@ -131,14 +133,15 @@
 class HtmlElementConfig(TypedDict):
     tag_omission: bool
     tag: str
 
 
 class BaseHtmlElement(ABC, metaclass=HtmlMetaClass):
     __html_subclasses__: ClassVar[List[Type["BaseHtmlElement"]]] = []
+    escape: bool = True
 
     # Defined on Metaclass
     if TYPE_CHECKING:
         __html_attributes__: ClassVar[Dict[str, HtmlAttributeInfo]]
         __html_config__: ClassVar[HtmlElementConfig]
 
     def __init_subclass__(cls, *_args: Any, **_kwargs: Any):
@@ -191,22 +194,22 @@
         for field, value in kwargs.items():
             setattr(self, field, value)
 
     def to_html(self, indent: int = 0, indent_step: int = 2, format: bool = True) -> str:
         # https://github.com/justpy-org/justpy/blob/master/justpy/htmlcomponents.py#L459C5-L474C17
         block_indent = " " * indent if format else ""
         endline = "\n" if format else ""
-        html_tag = self.get_config_value("tag")
+        html_tag = html.escape(str(self.get_config_value("tag")), quote=True)
         html_string = f"{block_indent}<{html_tag}"
 
         for key, attribute in self.__html_attributes__.items():
             if attribute.attribute_type != "attribute":
                 continue
             value = getattr(self, key, None)
-            new_attribute = format_attribute(key, value, attribute)
+            new_attribute = format_attribute(key, value, attribute, escape=self.escape)
             if new_attribute:
                 html_string += f" {new_attribute}"
 
         content: List[Tuple[Union[str, "BaseHtmlElement", Any], HtmlAttributeInfo]] = []
         for key, attribute in self.__html_attributes__.items():
             if attribute.attribute_type != "content":
                 continue
@@ -223,17 +226,18 @@
             html_string += f">{endline}"
             new_indent_amount = indent + indent_step if format else 0
             for c, attribute in content:
                 if isinstance(c, BaseHtmlElement):
                     html_string += c.to_html(indent=new_indent_amount, indent_step=indent_step, format=format)
                 else:
                     if attribute.transformer:
-                        value = attribute.transformer(c)
+                        value = str(attribute.transformer(c))
                     else:
                         value = str(c)
+                    value = html.escape(value, quote=True) if self.escape else value
                     new_indent = " " * new_indent_amount
                     html_string += f"{new_indent}{value}{endline}"
 
             html_string += f"{block_indent}</{html_tag}>{endline}"
         else:
             if self.get_config_value("tag_omission"):
                 html_string += f" />{endline}"
@@ -249,34 +253,36 @@
     def __str__(self) -> str:
         return self.to_html()
 
     def __repr__(self) -> str:
         return f"<{self.__html_config__['tag']}> field"
 
 
-def format_attribute(key: str, value: Any, attribute: HtmlAttributeInfo, inner_multi: bool = False) -> str:
+def format_attribute(key: str, value: Any, attribute: HtmlAttributeInfo, inner_multi: bool = False, escape: bool = True) -> str:
     """
     Formats the attribute to add to the html attributes.
     Depending on the value and attribute config, this can add zero, one or more attributes
     Returns the attribute to add e.g. `selected`, `type="button"` or `aria-type="button" aria-checked="false"`
     """
     html_attribute = attribute.html_attribute or key if not inner_multi else key
+    html_attribute = html.escape(html_attribute, quote=True) if escape else html_attribute
     if value is None:
         return ""
     if not inner_multi and attribute.multi_attribute:
         # For an aria dict, treat each value as
         formatted = [
-            format_attribute(f"{html_attribute}-{sub_key}", sub_value, attribute, inner_multi=True)
+            format_attribute(f"{html_attribute}-{sub_key}", sub_value, attribute, inner_multi=True, escape=escape)
             for sub_key, sub_value in value.items()
         ]
         # Don't add empty attributes
         return " ".join(i for i in formatted if i)
     if isinstance(value, bool):
         # for e.g. disabled. Only set if true
         if value:
-            return f"{html_attribute}"
+            return html_attribute
         return ""
-    if attribute.transformer:
+    elif attribute.transformer:
         value = attribute.transformer(value)
         if value == "":
             return ""
+    value = html.escape(str(value), quote=True) if escape else value
     return f'{html_attribute}="{value}"'
```

### Comparing `html_elements-0.1.4/html_elements/elements.py` & `html_elements-0.2.0/html_elements/elements.py`

 * *Files identical despite different names*

### Comparing `html_elements-0.1.4/html_elements/extensions.py` & `html_elements-0.2.0/html_elements/extensions.py`

 * *Files identical despite different names*

### Comparing `html_elements-0.1.4/pyproject.toml` & `html_elements-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "html-elements"
-version = "0.1.4"
+version = "0.2.0"
 description = "HTML element objects to use in pure Python server side rendering"
 authors = ["Anton De Meester <antondemeester@gmail.com>"]
 readme = "README.md"
 packages = [{include = "html_elements"}]
 license = "MIT"
 
 [project.urls]
```

### Comparing `html_elements-0.1.4/PKG-INFO` & `html_elements-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: html-elements
-Version: 0.1.4
+Version: 0.2.0
 Summary: HTML element objects to use in pure Python server side rendering
 License: MIT
 Author: Anton De Meester
 Author-email: antondemeester@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

