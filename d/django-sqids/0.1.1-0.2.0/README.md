# Comparing `tmp/django_sqids-0.1.1.tar.gz` & `tmp/django_sqids-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_sqids-0.1.1.tar", max compression
+gzip compressed data, was "django_sqids-0.2.0.tar", max compression
```

## Comparing `django_sqids-0.1.1.tar` & `django_sqids-0.2.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1098 2023-11-16 14:15:52.178118 django_sqids-0.1.1/LICENSE
--rw-r--r--   0        0        0     4662 2024-01-27 13:43:23.330938 django_sqids-0.1.1/README.md
--rw-r--r--   0        0        0       94 2023-11-16 14:15:52.178118 django_sqids-0.1.1/django_sqids/__init__.py
--rw-r--r--   0        0        0       97 2023-11-16 14:15:52.178118 django_sqids-0.1.1/django_sqids/exceptions.py
--rw-r--r--   0        0        0     5253 2024-01-27 13:34:36.190938 django_sqids-0.1.1/django_sqids/field.py
--rw-r--r--   0        0        0      826 2024-01-27 13:38:03.190938 django_sqids-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     5412 1970-01-01 00:00:00.000000 django_sqids-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1098 2023-11-16 11:28:24.617022 django_sqids-0.2.0/LICENSE
+-rw-r--r--   0        0        0     5686 2024-04-29 07:11:15.652554 django_sqids-0.2.0/README.md
+-rw-r--r--   0        0        0       94 2023-11-16 12:05:15.716429 django_sqids-0.2.0/django_sqids/__init__.py
+-rw-r--r--   0        0        0       97 2023-11-16 11:24:54.200828 django_sqids-0.2.0/django_sqids/exceptions.py
+-rw-r--r--   0        0        0     5729 2024-04-29 07:11:15.662556 django_sqids-0.2.0/django_sqids/field.py
+-rw-r--r--   0        0        0      862 2024-04-29 07:13:37.383923 django_sqids-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     6436 1970-01-01 00:00:00.000000 django_sqids-0.2.0/PKG-INFO
```

### Comparing `django_sqids-0.1.1/LICENSE` & `django_sqids-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django_sqids-0.1.1/README.md` & `django_sqids-0.2.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -9,21 +9,21 @@
 
 The project was forked from [django-hashids](https://github.com/ericls/django-hashids) to provide the same functionality with the newer Sqids library.
 
 # Features
 
 - Proxy the internal model `pk` field without storing the value in the database.
 - Allows lookups and filtering by sqid string.
-- Can be used as sort key
-- Allows specifying a min_length and alphabet globally
-- Supports custom min_length, and alphabet per field
-- Supports Django REST Framework Serializers
+- Can be used as sort key.
+- Allows specifying a min_length and alphabet globally.
+- Supports custom min_length, prefix, and alphabet per field.
+- Supports Django REST Framework Serializers.
 - Supports exact ID searches in Django Admin when field is specified in search_fields.
-- Supports common filtering lookups, such as `__iexact`, `__contains`, `__icontains`, though matching is the same as `__exact`.
-- Supports other lookups: isnull, gt, gte, lt and lte.
+- Supports filtering by `__iexact`, though matching is the same as `__exact`.
+- Supports other lookups: `in`, `isnull`, `gt`, `gte`, `lt`, and `lte`.
 
 # Install
 
 ```bash
 pip install django-sqids
 ```
 
@@ -59,15 +59,14 @@
 TestModel.objects.filter(sqid="1Z")
 TestModel.objects.filter(sqid__in=["1Z", "4x"])
 TestModel.objects.filter(sqid__gt="1Z")  # same as id__gt=1, would return instance 2
 
 # Allows usage in queryset.values
 TestModel.objects.values_list("sqid", flat=True) # ["1Z", "4x"]
 TestModel.objects.filter(sqid__in=TestModel.objects.values("sqid"))
-
 ```
 
 ## Using with URLs
 
 You can use sqids to identify items in your URLs by treating them as slugs.
 
 In `urls.py`:
@@ -95,36 +94,41 @@
     search_fields = [
         "sqid__exact",
     ]
 ```
 
 ## Config
 
-The folloing attributes can be added in settings file to set default arguments of `SqidsField`:
+The following attributes can be added in settings file to set default arguments of `SqidsField`:
 
 1. `DJANGO_SQIDS_MIN_LENGTH`: default minimum length
 2. `DJANGO_SQIDS_ALPHABET`: default alphabet
 
 `SqidsField` does not reqiure any arguments but the following arguments can be supplied to modify its behavior.
 
-| Name              |                       Description                       |
-| ----------------- | :-----------------------------------------------------: |
-| `real_field_name` |                 The proxied field name                  |
-| `sqids_instance`  | The sqids instance used to encode/decode for this field |
-| `min_length`      |  The minimum length of sqids generated for this field   |
-| `alphabet`        |    The alphabet used by this field to generate sqids    |
+| Name              |                       Description                       | Example                                                     |
+| ----------------- | :-----------------------------------------------------: | ----------------------------------------------------------- |
+| `real_field_name` |                 The proxied field name                  | sqid = SqidsField(real_field_name="id")                     |
+| `sqids_instance`  | The sqids instance used to encode/decode for this field | sqid = SqidsField(sqids_instance=sqids_instance)            |
+| `min_length`      |  The minimum length of sqids generated for this field   | sqid = SqidsField(min_length=10)                            |
+| `alphabet`        |    The alphabet used by this field to generate sqids    | sqid = SqidsField(alphabet="KHE5J3L2M4N6P7Q8R9T0V1W2X3Y4Z") |
+| `prefix`          |     The prefix used by this field to generate sqids     | sqid = SqidsField(prefix="item-")                           |
 
 The argument `sqids_instance` is mutually exclusive to `min_length` and `alphabet`. See [sqids-python](https://github.com/sqids/sqids-python) for more info about the arguments.
 
 Some common Model arguments such as `verbose_name` are also supported.
 
 ## Where did the Salt go?
 
-[Sqids removed the "salt" parameter](https://sqids.org/faq#salt) to prevent association with security or safety.
-`django_sqids` provides a useful `shuffle_alphabet` function that helps reintroduce the same idea:
+When the Hashids project transitioned to Sqids, [Sqids removed the "salt" parameter](https://sqids.org/faq#salt) to prevent the appearance that
+it provides security or safety. In Sqids, the order of the alphabet affects the generated sqids. `django_sqids` provides a useful `shuffle_alphabet` 
+function that helps reintroduce the same idea as the "salt" parameter by shuffling the alphabet. This can be used to generate a unique alphabet for each
+instance of `SqidsField` to prevent the same id from generating the same sqid across different instances of `SqidsField`.
+
+The `seed` parameter is used to generate a unique ordering of alphabet for each instance of `SqidsField`. The `alphabet` parameter can be used to specify a custom alphabet.
 
 ```python
 from django_sqids import SqidsField, shuffle_alphabet
 
 class MyModel(models.Model):
     # will use your configured default alphabet
     sqid = SqidsField(alphabet=shuffle_alphabet(seed='randomSeed'))
```

### Comparing `django_sqids-0.1.1/django_sqids/field.py` & `django_sqids-0.2.0/django_sqids/field.py`

 * *Files 8% similar despite different names*

```diff
@@ -32,21 +32,23 @@
     def __init__(
         self,
         real_field_name="id",
         *args,
         sqids_instance=None,
         alphabet=None,
         min_length=None,
-        **kwargs
+        prefix="",
+        **kwargs,
     ):
         kwargs.pop("editable", None)
         super().__init__(*args, editable=False, **kwargs)
         self.real_field_name = real_field_name
         self.min_length = min_length
         self.alphabet = alphabet
+        self.prefix = prefix
         self._explicit_sqids_instance = sqids_instance
 
         self.sqids_instance = None
         self.attached_to_model = None
 
     def contribute_to_class(self, cls, name):
         self.attname = name
@@ -89,21 +91,28 @@
         if alphabet is None:
             alphabet = (
                 getattr(settings, "DJANGO_SQIDS_ALPHABET", None) or DEFAULT_ALPHABET
             )
         return Sqids(min_length=min_length, alphabet=alphabet)
 
     def get_prep_value(self, value):
+        if self.prefix:
+            if value.startswith(self.prefix):
+                value = value[len(self.prefix) :]
+            else:
+                return None
         decoded_values = self.sqids_instance.decode(value)
         if not decoded_values:
             return None
         return decoded_values[0]
 
     def from_db_value(self, value, expression, connection, *args):
-        return self.sqids_instance.encode([value])
+        # Prepend the prefix when encoding for display
+        encoded_value = self.sqids_instance.encode([value])
+        return f"{self.prefix}{encoded_value}" if encoded_value is not None else None
 
     def get_col(self, alias, output_field=None):
         if output_field is None:
             output_field = self
         col = self.real_col.get_col(alias, output_field)
         return col
 
@@ -131,15 +140,17 @@
         if not instance:
             return self
         real_value = getattr(instance, self.real_field_name, None)
         # the instance is not saved yet?
         if real_value is None:
             return ""
         assert isinstance(real_value, int)
-        return self.sqids_instance.encode([real_value])
+        # Prepend the prefix when encoding for display
+        encoded_value = self.sqids_instance.encode([real_value])
+        return f"{self.prefix}{encoded_value}"
 
     def __set__(self, instance, value):
         pass
 
     def __deepcopy__(self, memo=None):
         new_instance = super().__deepcopy__(memo)
         for attr in ("sqids_instance", "attached_to_model"):
```

### Comparing `django_sqids-0.1.1/pyproject.toml` & `django_sqids-0.2.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 [tool.poetry]
 name = "django-sqids"
-version = "0.1.1"
+version = "0.2.0"
 readme = "README.md"
 description = "Non-intrusive sqids library for Django"
 homepage = "https://github.com/julianwachholz/django-sqids"
 repository = "https://github.com/julianwachholz/django-sqids"
 keywords = ["django", "sqids", "sqid", "hashids", "hashid"]
 authors = ["Julian Wachholz <julian@wachholz.ch>", "Shen Li <dustet@gmail.com>"]
 license = "MIT"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4"
 sqids = ">=0.4.1"
 
 [tool.poetry.group.dev.dependencies]
 django = [
-  { version = "^4.2.7", python = ">=3.8.1,<3.10" },
-  { version = "^5.0.1", python = ">=3.10" },
+    { version = "^4.2.7", python = ">=3.8.1,<3.10" },
+    { version = "^5.0.1", python = ">=3.10" },
 ]
 black = "^23.11.0"
 flake8 = "^6.1.0"
 isort = "^5.12.0"
 pytest = "^7.4.3"
 pytest-cov = "^4.1.0"
 pytest-django = "^4.7.0"
+djangorestframework = "^3.14.0"
 
 [build-system]
 requires = ["poetry>=0.12"]
 build-backend = "poetry.masonry.api"
```

### Comparing `django_sqids-0.1.1/PKG-INFO` & `django_sqids-0.2.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-sqids
-Version: 0.1.1
+Version: 0.2.0
 Summary: Non-intrusive sqids library for Django
 Home-page: https://github.com/julianwachholz/django-sqids
 License: MIT
 Keywords: django,sqids,sqid,hashids,hashid
 Author: Julian Wachholz
 Author-email: julian@wachholz.ch
 Requires-Python: >=3.8.1,<4
@@ -29,21 +29,21 @@
 
 The project was forked from [django-hashids](https://github.com/ericls/django-hashids) to provide the same functionality with the newer Sqids library.
 
 # Features
 
 - Proxy the internal model `pk` field without storing the value in the database.
 - Allows lookups and filtering by sqid string.
-- Can be used as sort key
-- Allows specifying a min_length and alphabet globally
-- Supports custom min_length, and alphabet per field
-- Supports Django REST Framework Serializers
+- Can be used as sort key.
+- Allows specifying a min_length and alphabet globally.
+- Supports custom min_length, prefix, and alphabet per field.
+- Supports Django REST Framework Serializers.
 - Supports exact ID searches in Django Admin when field is specified in search_fields.
-- Supports common filtering lookups, such as `__iexact`, `__contains`, `__icontains`, though matching is the same as `__exact`.
-- Supports other lookups: isnull, gt, gte, lt and lte.
+- Supports filtering by `__iexact`, though matching is the same as `__exact`.
+- Supports other lookups: `in`, `isnull`, `gt`, `gte`, `lt`, and `lte`.
 
 # Install
 
 ```bash
 pip install django-sqids
 ```
 
@@ -79,15 +79,14 @@
 TestModel.objects.filter(sqid="1Z")
 TestModel.objects.filter(sqid__in=["1Z", "4x"])
 TestModel.objects.filter(sqid__gt="1Z")  # same as id__gt=1, would return instance 2
 
 # Allows usage in queryset.values
 TestModel.objects.values_list("sqid", flat=True) # ["1Z", "4x"]
 TestModel.objects.filter(sqid__in=TestModel.objects.values("sqid"))
-
 ```
 
 ## Using with URLs
 
 You can use sqids to identify items in your URLs by treating them as slugs.
 
 In `urls.py`:
@@ -115,36 +114,41 @@
     search_fields = [
         "sqid__exact",
     ]
 ```
 
 ## Config
 
-The folloing attributes can be added in settings file to set default arguments of `SqidsField`:
+The following attributes can be added in settings file to set default arguments of `SqidsField`:
 
 1. `DJANGO_SQIDS_MIN_LENGTH`: default minimum length
 2. `DJANGO_SQIDS_ALPHABET`: default alphabet
 
 `SqidsField` does not reqiure any arguments but the following arguments can be supplied to modify its behavior.
 
-| Name              |                       Description                       |
-| ----------------- | :-----------------------------------------------------: |
-| `real_field_name` |                 The proxied field name                  |
-| `sqids_instance`  | The sqids instance used to encode/decode for this field |
-| `min_length`      |  The minimum length of sqids generated for this field   |
-| `alphabet`        |    The alphabet used by this field to generate sqids    |
+| Name              |                       Description                       | Example                                                     |
+| ----------------- | :-----------------------------------------------------: | ----------------------------------------------------------- |
+| `real_field_name` |                 The proxied field name                  | sqid = SqidsField(real_field_name="id")                     |
+| `sqids_instance`  | The sqids instance used to encode/decode for this field | sqid = SqidsField(sqids_instance=sqids_instance)            |
+| `min_length`      |  The minimum length of sqids generated for this field   | sqid = SqidsField(min_length=10)                            |
+| `alphabet`        |    The alphabet used by this field to generate sqids    | sqid = SqidsField(alphabet="KHE5J3L2M4N6P7Q8R9T0V1W2X3Y4Z") |
+| `prefix`          |     The prefix used by this field to generate sqids     | sqid = SqidsField(prefix="item-")                           |
 
 The argument `sqids_instance` is mutually exclusive to `min_length` and `alphabet`. See [sqids-python](https://github.com/sqids/sqids-python) for more info about the arguments.
 
 Some common Model arguments such as `verbose_name` are also supported.
 
 ## Where did the Salt go?
 
-[Sqids removed the "salt" parameter](https://sqids.org/faq#salt) to prevent association with security or safety.
-`django_sqids` provides a useful `shuffle_alphabet` function that helps reintroduce the same idea:
+When the Hashids project transitioned to Sqids, [Sqids removed the "salt" parameter](https://sqids.org/faq#salt) to prevent the appearance that
+it provides security or safety. In Sqids, the order of the alphabet affects the generated sqids. `django_sqids` provides a useful `shuffle_alphabet` 
+function that helps reintroduce the same idea as the "salt" parameter by shuffling the alphabet. This can be used to generate a unique alphabet for each
+instance of `SqidsField` to prevent the same id from generating the same sqid across different instances of `SqidsField`.
+
+The `seed` parameter is used to generate a unique ordering of alphabet for each instance of `SqidsField`. The `alphabet` parameter can be used to specify a custom alphabet.
 
 ```python
 from django_sqids import SqidsField, shuffle_alphabet
 
 class MyModel(models.Model):
     # will use your configured default alphabet
     sqid = SqidsField(alphabet=shuffle_alphabet(seed='randomSeed'))
```

