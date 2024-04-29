# Comparing `tmp/drf_serializer_dumps-1.0.0.tar.gz` & `tmp/drf_serializer_dumps-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drf_serializer_dumps-1.0.0.tar", last modified: Sun Apr 21 18:13:43 2024, max compression
+gzip compressed data, was "drf_serializer_dumps-1.0.1.tar", last modified: Mon Apr 29 21:14:03 2024, max compression
```

## Comparing `drf_serializer_dumps-1.0.0.tar` & `drf_serializer_dumps-1.0.1.tar`

### file list

```diff
@@ -1,16 +1,30 @@
-drwxrwxrwx   0        0        0        0 2024-04-21 18:13:43.181548 drf_serializer_dumps-1.0.0/
--rw-rw-rw-   0        0        0     1085 2024-04-16 14:24:28.000000 drf_serializer_dumps-1.0.0/LICENSE
--rw-rw-rw-   0        0        0       89 2024-04-16 20:59:30.000000 drf_serializer_dumps-1.0.0/MANIFEST.in
--rw-rw-rw-   0        0        0     4087 2024-04-21 18:13:43.180547 drf_serializer_dumps-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     2418 2024-04-18 10:24:51.000000 drf_serializer_dumps-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2024-04-21 18:13:43.172546 drf_serializer_dumps-1.0.0/drf_serializer_dumps/
--rw-rw-rw-   0        0        0        0 2024-04-16 21:11:45.000000 drf_serializer_dumps-1.0.0/drf_serializer_dumps/__init__.py
--rw-rw-rw-   0        0        0    10239 2024-04-18 10:25:09.000000 drf_serializer_dumps-1.0.0/drf_serializer_dumps/decorators.py
-drwxrwxrwx   0        0        0        0 2024-04-21 18:13:43.179546 drf_serializer_dumps-1.0.0/drf_serializer_dumps.egg-info/
--rw-rw-rw-   0        0        0     4087 2024-04-21 18:13:43.000000 drf_serializer_dumps-1.0.0/drf_serializer_dumps.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      325 2024-04-21 18:13:43.000000 drf_serializer_dumps-1.0.0/drf_serializer_dumps.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-21 18:13:43.000000 drf_serializer_dumps-1.0.0/drf_serializer_dumps.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       67 2024-04-21 18:13:43.000000 drf_serializer_dumps-1.0.0/drf_serializer_dumps.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2024-04-21 18:13:43.000000 drf_serializer_dumps-1.0.0/drf_serializer_dumps.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-21 18:13:43.181548 drf_serializer_dumps-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1418 2024-04-17 08:19:03.000000 drf_serializer_dumps-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 21:14:03.618229 drf_serializer_dumps-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-04-29 21:13:58.000000 drf_serializer_dumps-1.0.1/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 21:14:03.610229 drf_serializer_dumps-1.0.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 21:14:03.614230 drf_serializer_dumps-1.0.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     3771 2024-04-29 21:13:58.000000 drf_serializer_dumps-1.0.1/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-29 21:13:58.000000 drf_serializer_dumps-1.0.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1576 2024-04-29 21:13:58.000000 drf_serializer_dumps-1.0.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3899 2024-04-29 21:13:58.000000 drf_serializer_dumps-1.0.1/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-29 21:13:58.000000 drf_serializer_dumps-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    11584 2024-04-29 21:14:03.618229 drf_serializer_dumps-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8350 2024-04-29 21:13:58.000000 drf_serializer_dumps-1.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)    12285 2024-04-29 21:13:58.000000 drf_serializer_dumps-1.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 21:14:03.618229 drf_serializer_dumps-1.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 21:14:03.610229 drf_serializer_dumps-1.0.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 21:14:03.614230 drf_serializer_dumps-1.0.1/src/drf_serializer_dumps/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 21:13:58.000000 drf_serializer_dumps-1.0.1/src/drf_serializer_dumps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9949 2024-04-29 21:13:58.000000 drf_serializer_dumps-1.0.1/src/drf_serializer_dumps/decorators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 21:14:03.614230 drf_serializer_dumps-1.0.1/src/drf_serializer_dumps.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11584 2024-04-29 21:14:03.000000 drf_serializer_dumps-1.0.1/src/drf_serializer_dumps.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      599 2024-04-29 21:14:03.000000 drf_serializer_dumps-1.0.1/src/drf_serializer_dumps.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 21:14:03.000000 drf_serializer_dumps-1.0.1/src/drf_serializer_dumps.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-29 21:14:03.000000 drf_serializer_dumps-1.0.1/src/drf_serializer_dumps.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      244 2024-04-29 21:14:03.000000 drf_serializer_dumps-1.0.1/src/drf_serializer_dumps.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-29 21:14:03.000000 drf_serializer_dumps-1.0.1/src/drf_serializer_dumps.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 21:14:03.614230 drf_serializer_dumps-1.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 21:13:58.000000 drf_serializer_dumps-1.0.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-29 21:13:58.000000 drf_serializer_dumps-1.0.1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-04-29 21:13:58.000000 drf_serializer_dumps-1.0.1/tests/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-04-29 21:13:58.000000 drf_serializer_dumps-1.0.1/tests/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1316 2024-04-29 21:13:58.000000 drf_serializer_dumps-1.0.1/tests/test_decorators.py
```

### Comparing `drf_serializer_dumps-1.0.0/drf_serializer_dumps/decorators.py` & `drf_serializer_dumps-1.0.1/src/drf_serializer_dumps/decorators.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,249 +1,242 @@
-from __future__ import annotations
-import json
-from datetime import date, datetime, time, timedelta
-from types import UnionType
-from typing import (
-    TYPE_CHECKING,
-    Any,
-    Union,
-    get_args,
-    get_origin,
-    get_type_hints,
-)
-from uuid import UUID, uuid4
-
-from django.utils import timezone
-from drf_spectacular.utils import OpenApiTypes
-from rest_framework import serializers
-
-if TYPE_CHECKING:
-    from collections import OrderedDict
-
-__all__ = ('serializer_dumps',)
-
-SerializerType = serializers.Serializer | type[serializers.Serializer]
-
-_uuid = uuid4()
-_now = timezone.now()
-
-
-def serializer_dumps(
-    klass: SerializerType,
-    exclude_fields: list[str] | None = None,
-    renew_type_value: bool = False,
-    extend_type_map: dict[type, Any] | None = None,
-) -> dict[str, Any]:
-    """
-    - Генерирует `Example Value` для `Swagger` на основе класса сериализатора,\
-    используя названия полей, классы полей, и типы полей.
-    - Так же ищет типы в декораторе `@extend_schema_field` с `OpenApiTypes` типами.
-    - Если метод у `SerializerMethodField` возвращает вложенный сериализатор,\
-    то в качестве `type hints` необходимо указать класс этого сериализатора.
-    #### Пример 1::
-
-        class PersonCars(serializers.Serializer):
-            car_name = serializers.CharField()
-            car_price = serializers.IntegerField()
-
-        class PersonSerializer(serializers.Serializer):
-            name = serializers.CharField()
-            age = serializers.IntegerField()
-            cars = PersonCars(many=True)
-        -----------------------------------------------
-        serializer_dumps(PersonSerializer)
-        {'name': 'string', 'age': 1, 'cars': [{'car_name': 'string', 'car_price': 1}]}
-
-    #### Пример 2::
-
-        class Person(models.Model):
-            name = models.CharField(max_length=256)
-            phones = ArrayField(models.CharField(max_length=256))
-
-        class PersonSerializer(serializers.ModelSerializer):
-            class Meta:
-                model = Person
-                fields = '__all__'
-        -----------------------------------------------
-        serializer_dumps(PersonSerializer)
-        {'name': 'string', 'phones': ['string']}
-
-    #### Integration with drf-spectacular extend_schema decorator::
-
-        @extend_schema(
-            examples=[
-                OpenApiExample('Name1', serializer_dumps(Some1Serializer)),
-                OpenApiExample('Name2', serializer_dumps(Some2Serializer)),
-            ]
-        )
-        def your_api_method(self, request, *args, **kwargs):
-            ...
-
-    - Необязательные параметры:
-        - `exclude_fields` Исключить ряд полей сериализатора при генерации словаря.
-        - `renew_type_value` Генерировать новый `uuid` и `datetime, date, time` при вызове функции.
-        - `extend_type_map` Расширить словарь типов к значениям по умолчанию,\
-        новыми типами и их значениями, либо переопределить уже существующие типы и их значения.
-    """
-    if exclude_fields is None:
-        exclude_fields = []
-    if extend_type_map is None:
-        extend_type_map = {}
-
-    if renew_type_value:
-        global _uuid
-        global _now
-        _uuid = uuid4()
-        _now = timezone.now()
-
-    field_type_mapping = {
-        serializers.CharField: 'string',
-        serializers.FloatField: 1.0,
-        serializers.BooleanField: False,
-        serializers.IntegerField: 1,
-        serializers.UUIDField: _uuid,
-        serializers.DateTimeField: _now,
-        serializers.DateField: _now.date(),
-        serializers.TimeField: _now.time(),
-        serializers.DurationField: timedelta(seconds=5),
-    }
-    reversed_field_type_mapping = {value: field for field, value in field_type_mapping.items()}
-    type_mapping = {
-        **field_type_mapping,
-        OpenApiTypes.STR: 'string',
-        OpenApiTypes.DOUBLE: 1.0,
-        OpenApiTypes.BOOL: False,
-        OpenApiTypes.BINARY: b'string',
-        OpenApiTypes.INT: 1,
-        OpenApiTypes.UUID: _uuid,
-        OpenApiTypes.DATETIME: _now,
-        OpenApiTypes.DATE: _now.date(),
-        OpenApiTypes.TIME: _now.time(),
-        OpenApiTypes.DURATION: timedelta(seconds=5),
-        OpenApiTypes.OBJECT: {},
-        OpenApiTypes.ANY: {},
-        OpenApiTypes.NONE: None,
-        str: 'string',
-        float: 1.0,
-        bool: False,
-        bytes: b'string',
-        int: 1,
-        UUID: _uuid,
-        datetime: _now,
-        date: _now.date(),
-        time: _now.time(),
-        timedelta: timedelta(seconds=5),
-        dict: {},
-        Any: {},
-        None: None,
-        **extend_type_map,
-    }
-
-    def _get_type_value(
-        klass: SerializerType,
-        field_name: str,
-        field_instance: serializers.SerializerMethodField,
-    ) -> tuple[Any, type]:
-        """
-        Получить типизацию у метода SerializerMethodField
-        """
-        if field_instance.method_name is None:
-            method = getattr(klass, f'get_{field_name}')
-        else:
-            method = getattr(klass, field_instance.method_name)
-
-        open_api_type = getattr(method, '_spectacular_annotation', {}).get('field')
-
-        # annotation = inspect.signature(method).return_annotation
-        # annotation = None if annotation is inspect._empty else annotation
-
-        annotation = get_type_hints(method).get('return')
-
-        # origin = get_origin(annotation)
-        # if origin is Union or origin is UnionType:
-        if get_origin(annotation) in (Union, UnionType):
-            annotation = get_args(annotation)[0]
-
-        type_value = type_mapping.get(open_api_type)
-        if type_value is None:
-            type_value = type_mapping.get(annotation)
-
-        return type_value, annotation
-
-    def _walk_fields_recursively(
-        klass: SerializerType, exclude_fields: list[str] | None = None
-    ) -> dict[str, Any]:
-        """
-        Рекурсивно проходит по всем полям и вложенным сериализаторам
-        для генерации `Example Value`.
-        """
-        if exclude_fields is None:
-            exclude_fields = []
-
-        fields: OrderedDict[str, SerializerType] = klass().get_fields()
-        example_val = {}
-
-        for field_name, field_instance in fields.items():
-            if field_name in exclude_fields:
-                continue
-
-            if isinstance(field_instance, serializers.ListSerializer):
-                nested_dict = _walk_fields_recursively(type(field_instance.child), exclude_fields)
-                example_val[field_name] = [nested_dict] if field_instance.many else nested_dict
-
-            elif isinstance(field_instance, serializers.ListField):  # support for postgres ArrayField
-                example_val[field_name] = [type_mapping.get(type(field_instance.child))]
-
-            elif not isinstance(field_instance, serializers.SerializerMethodField):
-                base_field_cls = type(field_instance).__bases__[0]  # __mro__
-                if base_field_cls is not serializers.Field and not issubclass(
-                    base_field_cls, serializers.Serializer
-                ):
-                    example_val[field_name] = base_field_cls().to_representation(
-                        type_mapping.get(base_field_cls)
-                    )
-                elif isinstance(field_instance, serializers.Serializer):
-                    example_val[field_name] = _walk_fields_recursively(
-                        type(field_instance), exclude_fields
-                    )
-                else:
-                    example_val[field_name] = field_instance.to_representation(
-                        type_mapping.get(type(field_instance))
-                    )
-
-            elif isinstance(field_instance, serializers.SerializerMethodField):
-                type_value, annotation = _get_type_value(klass, field_name, field_instance)
-
-                if type_value is not None:
-                    _field_instance = reversed_field_type_mapping.get(type_value)
-
-                    if _field_instance is not None:
-                        example_val[field_name] = _field_instance().to_representation(type_value)
-                    else:
-                        example_val[field_name] = type_value
-                        print(
-                            f'Обнаружена неизвестная аннотация: "{annotation.__name__}" '
-                            f'у поля: "{field_name}".'
-                        )
-                else:
-                    if issubclass(annotation, serializers.Serializer):
-                        example_val[field_name] = _walk_fields_recursively(annotation, exclude_fields)
-                    else:
-                        example_val[field_name] = None
-                        print(
-                            f'Обнаружена неизвестная аннотация: "{annotation.__name__}" '
-                            f'Для поля: "{field_name}" было установлено значение "None".'
-                        )
-            else:
-                example_val[field_name] = None
-                print(
-                    f'Обнаружено неизвестное поле: "{type(field_instance).__name__}" '
-                    f'Для поля: "{field_name}" было установлено значение "None".'
-                )
-
-        return example_val
-
-    return json.loads(
-        json.dumps(
-            _walk_fields_recursively(klass, exclude_fields), ensure_ascii=False, default=str, indent=4
-        )
-    )
+from __future__ import annotations
+
+import json
+from datetime import date, datetime, time, timedelta
+from typing import TYPE_CHECKING, Any, Union, get_args, get_origin, get_type_hints
+from uuid import UUID, uuid4
+
+from django.utils import timezone
+from drf_spectacular.types import OpenApiTypes
+from rest_framework import serializers
+
+if TYPE_CHECKING:
+    from collections import OrderedDict
+
+    from drf_spectacular.utils import _SerializerType
+
+__all__ = ('serializer_dumps',)
+
+_uuid = uuid4()
+_now = timezone.now()
+
+
+def serializer_dumps(
+    klass: _SerializerType,
+    exclude_fields: list[str] | None = None,
+    renew_type_value: bool = False,
+    extend_type_map: dict[type, Any] | None = None,
+) -> dict[str, Any]:
+    """
+    - Генерирует `Example Value` для `Swagger` на основе класса сериализатора,\
+    используя названия полей, классы полей, и типы полей.
+    - Так же ищет типы в декораторе `@extend_schema_field` с `OpenApiTypes` типами.
+    - Если метод у `SerializerMethodField` возвращает вложенный сериализатор,\
+    то в качестве `type hints` необходимо указать класс этого сериализатора.
+    #### Пример 1::
+
+        class PersonCars(serializers.Serializer):
+            car_name = serializers.CharField()
+            car_price = serializers.IntegerField()
+
+        class PersonSerializer(serializers.Serializer):
+            name = serializers.CharField()
+            age = serializers.IntegerField()
+            cars = PersonCars(many=True)
+        -----------------------------------------------
+        serializer_dumps(PersonSerializer)
+        {'name': 'string', 'age': 1, 'cars': [{'car_name': 'string', 'car_price': 1}]}
+
+    #### Пример 2::
+
+        class Person(models.Model):
+            name = models.CharField(max_length=256)
+            phones = ArrayField(models.CharField(max_length=256))
+
+        class PersonSerializer(serializers.ModelSerializer):
+            class Meta:
+                model = Person
+                fields = '__all__'
+        -----------------------------------------------
+        serializer_dumps(PersonSerializer)
+        {'id': 1, 'name': 'string', 'phones': ['string']}
+
+    #### Integration with drf-spectacular extend_schema decorator::
+
+        @extend_schema(
+            examples=[
+                OpenApiExample('Name1', serializer_dumps(Some1Serializer)),
+                OpenApiExample('Name2', serializer_dumps(Some2Serializer)),
+            ]
+        )
+        def your_api_method(self, request, *args, **kwargs):
+            ...
+
+    - Необязательные параметры:
+        - `exclude_fields` Исключить ряд полей сериализатора при генерации словаря.
+        - `renew_type_value` Генерировать новый `uuid` и `datetime, date, time` при вызове функции.
+        - `extend_type_map` Расширить словарь типов к значениям по умолчанию,\
+        новыми типами и их значениями, либо переопределить уже существующие типы и их значения.
+    """
+    if exclude_fields is None:
+        exclude_fields = []
+    if extend_type_map is None:
+        extend_type_map = {}
+
+    if renew_type_value:
+        global _uuid
+        global _now
+        _uuid = uuid4()
+        _now = timezone.now()
+
+    field_type_mapping = {
+        serializers.CharField: 'string',
+        serializers.FloatField: 1.0,
+        serializers.BooleanField: False,
+        serializers.IntegerField: 1,
+        serializers.UUIDField: _uuid,
+        serializers.DateTimeField: _now,
+        serializers.DateField: _now.date(),
+        serializers.TimeField: _now.time(),
+        serializers.DurationField: timedelta(seconds=5),
+    }
+    reversed_field_type_mapping = {value: field for field, value in field_type_mapping.items()}
+    type_mapping = {
+        **field_type_mapping,
+        OpenApiTypes.STR: 'string',
+        OpenApiTypes.DOUBLE: 1.0,
+        OpenApiTypes.BOOL: False,
+        OpenApiTypes.BINARY: b'string',
+        OpenApiTypes.INT: 1,
+        OpenApiTypes.UUID: _uuid,
+        OpenApiTypes.DATETIME: _now,
+        OpenApiTypes.DATE: _now.date(),
+        OpenApiTypes.TIME: _now.time(),
+        OpenApiTypes.DURATION: timedelta(seconds=5),
+        OpenApiTypes.OBJECT: {},
+        OpenApiTypes.ANY: {},
+        OpenApiTypes.NONE: None,
+        str: 'string',
+        float: 1.0,
+        bool: False,
+        bytes: b'string',
+        int: 1,
+        UUID: _uuid,
+        datetime: _now,
+        date: _now.date(),
+        time: _now.time(),
+        timedelta: timedelta(seconds=5),
+        dict: {},
+        Any: {},
+        None: None,
+        **extend_type_map,
+    }
+
+    def _get_type_value(
+        klass: _SerializerType,
+        field_name: str,
+        field_instance: serializers.SerializerMethodField,
+    ) -> tuple[Any, Any]:
+        """
+        Получить типизацию у метода SerializerMethodField
+        """
+        if field_instance.method_name is None:
+            method = getattr(klass, f'get_{field_name}')
+        else:
+            method = getattr(klass, field_instance.method_name)
+
+        open_api_type = getattr(method, '_spectacular_annotation', {}).get('field')
+
+        # annotation = inspect.signature(method).return_annotation
+        # annotation = None if annotation is inspect._empty else annotation
+
+        annotation = get_type_hints(method).get('return')
+
+        # origin = get_origin(annotation)
+        # if origin is Union or origin is type(Union):
+        if get_origin(annotation) in (Union, type(Union)):
+            annotation = get_args(annotation)[0]
+
+        type_value = type_mapping.get(open_api_type)
+        if type_value is None:
+            type_value = type_mapping.get(annotation)
+
+        return type_value, annotation
+
+    def _walk_fields_recursively(
+        klass: _SerializerType, exclude_fields: list[str] | None = None
+    ) -> dict[str, Any]:
+        """
+        Рекурсивно проходит по всем полям и вложенным сериализаторам
+        для генерации `Example Value`.
+        """
+        if exclude_fields is None:
+            exclude_fields = []
+
+        fields: OrderedDict[str, _SerializerType] = klass().get_fields()
+        example_val: dict[str, Any] = {}
+
+        for field_name, field_instance in fields.items():
+            if field_name in exclude_fields:
+                continue
+
+            if isinstance(field_instance, serializers.ListSerializer):
+                nested_dict = _walk_fields_recursively(type(field_instance.child), exclude_fields)
+                example_val[field_name] = [nested_dict] if field_instance.many else nested_dict
+
+            elif isinstance(field_instance, serializers.ListField):  # support for postgres ArrayField
+                example_val[field_name] = [type_mapping.get(type(field_instance.child))]
+
+            elif not isinstance(field_instance, serializers.SerializerMethodField):
+                base_field_cls = type(field_instance).__bases__[0]  # __mro__
+                if base_field_cls is not serializers.Field and not issubclass(
+                    base_field_cls, serializers.Serializer
+                ):
+                    example_val[field_name] = base_field_cls().to_representation(
+                        type_mapping.get(base_field_cls)
+                    )
+                elif isinstance(field_instance, serializers.Serializer):
+                    example_val[field_name] = _walk_fields_recursively(
+                        type(field_instance), exclude_fields
+                    )
+                else:
+                    example_val[field_name] = field_instance.to_representation(
+                        type_mapping.get(type(field_instance))
+                    )
+
+            elif isinstance(field_instance, serializers.SerializerMethodField):
+                type_value, annotation = _get_type_value(klass, field_name, field_instance)
+
+                if type_value is not None:
+                    _field_instance = reversed_field_type_mapping.get(type_value)
+
+                    if _field_instance is not None:
+                        example_val[field_name] = _field_instance().to_representation(type_value)
+                    else:
+                        example_val[field_name] = type_value
+                        print(
+                            f'Обнаружена неизвестная аннотация: "{annotation.__name__}" '
+                            f'у поля: "{field_name}".'
+                        )
+                else:
+                    if issubclass(annotation, serializers.Serializer):
+                        example_val[field_name] = _walk_fields_recursively(annotation, exclude_fields)
+                    else:
+                        example_val[field_name] = None
+                        print(
+                            f'Обнаружена неизвестная аннотация: "{annotation.__name__}" '
+                            f'Для поля: "{field_name}" было установлено значение "None".'
+                        )
+            else:
+                example_val[field_name] = None
+                print(
+                    f'Обнаружено неизвестное поле: "{type(field_instance).__name__}" '
+                    f'Для поля: "{field_name}" было установлено значение "None".'
+                )
+
+        return example_val
+
+    return json.loads(
+        json.dumps(
+            _walk_fields_recursively(klass, exclude_fields), ensure_ascii=False, default=str, indent=4
+        )
+    )
```

