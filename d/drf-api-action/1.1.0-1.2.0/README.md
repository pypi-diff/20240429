# Comparing `tmp/drf_api_action-1.1.0.tar.gz` & `tmp/drf_api_action-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drf_api_action-1.1.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "drf_api_action-1.2.0.tar", max compression
```

## Comparing `drf_api_action-1.1.0.tar` & `drf_api_action-1.2.0.tar`

### file list

```diff
@@ -1,11 +1,8 @@
--rw-r--r--   0        0        0     1068 2023-06-30 14:05:51.107400 drf_api_action-1.1.0/LICENSE.txt
--rw-r--r--   0        0        0     7472 2024-01-01 12:45:23.301769 drf_api_action-1.1.0/README.md
--rw-r--r--   0        0        0        0 2023-12-31 11:07:58.025649 drf_api_action-1.1.0/drf_api_action/__init__.py
--rw-r--r--   0        0        0     1092 2024-01-01 12:45:23.303434 drf_api_action-1.1.0/drf_api_action/api_utils.py
--rw-r--r--   0        0        0     3125 2024-01-01 12:45:23.304187 drf_api_action-1.1.0/drf_api_action/decorators.py
--rw-r--r--   0        0        0      320 2023-11-27 08:33:36.127871 drf_api_action-1.1.0/drf_api_action/exceptions.py
--rw-r--r--   0        0        0      831 2024-01-01 12:45:23.304805 drf_api_action-1.1.0/drf_api_action/fixtures.py
--rw-r--r--   0        0        0      856 2023-12-30 17:05:16.841747 drf_api_action-1.1.0/drf_api_action/mixins.py
--rw-r--r--   0        0        0     1453 2023-11-28 18:48:35.833423 drf_api_action-1.1.0/drf_api_action/utils.py
--rw-r--r--   0        0        0     4922 2024-01-01 12:48:46.549496 drf_api_action-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     8383 1970-01-01 00:00:00.000000 drf_api_action-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     4913 2024-04-29 15:06:56.791408 drf_api_action-1.2.0/README.md
+-rw-r--r--   0        0        0        0 2023-12-31 11:07:58.025649 drf_api_action-1.2.0/drf_api_action/__init__.py
+-rw-r--r--   0        0        0      320 2023-11-27 08:33:36.127871 drf_api_action-1.2.0/drf_api_action/exceptions.py
+-rw-r--r--   0        0        0      856 2023-12-30 17:05:16.841747 drf_api_action-1.2.0/drf_api_action/mixins.py
+-rw-r--r--   0        0        0     1169 2024-04-29 15:06:56.792375 drf_api_action-1.2.0/drf_api_action/plugin.py
+-rw-r--r--   0        0        0     2587 2024-04-29 15:06:56.793606 drf_api_action-1.2.0/drf_api_action/utils.py
+-rw-r--r--   0        0        0     5403 2024-04-29 15:06:56.794512 drf_api_action-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     6308 1970-01-01 00:00:00.000000 drf_api_action-1.2.0/PKG-INFO
```

### Comparing `drf_api_action-1.1.0/README.md` & `drf_api_action-1.2.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,36 +1,59 @@
+Metadata-Version: 2.1
+Name: drf_api_action
+Version: 1.2.0
+Summary: drf-api-action elevates DRF testing by simplifying REST endpoint testing to a seamless, function-like experience.
+Home-page: https://github.com/Ori-Roza/drf-api-action
+License: MIT
+Keywords: pytest,mocks,testing,fixtures,tests,django
+Author: Ori Roza
+Author-email: ori75660@gmail.com
+Requires-Python: >=3.7,<4.0
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Framework :: Pytest
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Topic :: Software Development :: Testing
+Requires-Dist: Django (>=4.2.8)
+Requires-Dist: djangorestframework (>=3.14.0)
+Requires-Dist: importlib_metadata (>=4.5.0,<5.0.0) ; python_version < "3.8"
+Requires-Dist: pytest-cov (==4.1.0)
+Requires-Dist: pytest-django (>=4.5.2)
+Project-URL: Repository, https://github.com/Ori-Roza/drf-api-action
+Description-Content-Type: text/markdown
+
 ![Alt text](resources/drf-api-action-banner-current.png?raw=true "")
 
 [![codecov](https://codecov.io/gh/Ori-Roza/drf-api-action/graph/badge.svg?token=2PB7NG8A4W)](https://codecov.io/gh/Ori-Roza/drf-api-action)
 [![python - 3.8 | 3.9 | 3.10 | 3.11](https://img.shields.io/badge/python-3.8_|_3.9_|_3.10_|_3.11-blue)](https://)[![CI](https://github.com/Ori-Roza/drf-api-action/actions/workflows/tests.yaml/badge.svg?branch=master)](https://github.com/Ori-Roza/drf-api-action/actions/workflows/tests.yaml)
 [![license - MIT](https://img.shields.io/badge/license-MIT-yellow)](https://)
 
 
 The drf-api-action Python package is designed to elevate your testing experience for Django Rest Framework (DRF) REST endpoints.
-With the custom decorator api-action, this package empowers you to effortlessly test your REST endpoints as if they were conventional functions.
+With the api-action fixture, this package empowers you to effortlessly test your REST endpoints as if they were conventional functions.
 
 Features:
 
 * **Simplified Testing:** Testing DRF REST endpoints using the api-action decorator, treating them like regular functions.
 
 * **Seamless Integration:** Replacing DRF's action decorator with api-action in your WebViewSet seamlessly.
 
 * **Clear Traceback:** Instead of getting a response with error code, get the real traceback that led to the error.
 
 * **Pagination Support**: Paginating easily through pages by a single kwarg.
 
-This package was designed in a way that you can use it in the following ways:
-
-* As a pytest fixture
-
-* As part of your ViewSet implementation
-
-## Demo
-
-![Alt Text](resources/drf-api-action-usage.gif?raw=true "")
 
 ## Installation
 
 You can install `drf-api-action` using pip:
 
 ```shell
 pip install drf-api-action
@@ -40,123 +63,66 @@
 
 ### To use `drf-api-action` as a Pytest fixture, you need to follow these steps:
 
 #### Step 1: Import the Required Classes and our fixture
 
 ```python
 import pytest
-from tests.test_app.models import DummyModel
-from tests.test_app.views import DummyViewSetFixture
-from drf_api_action.fixtures import action_api
+from tests.test_server.test_app.models import DummyModel
+from tests.test_server.test_app.views import DummyViewSetFixture
 ```
 
 #### Step 2: use the following action_api mark decorator:
 
 `@pytest.mark.action_api(view_set_class={YOUR VIEW_SET})`
 
 e.g:
 our ViewSet is called `DummyViewSetFixture`
+
 ```python
+import pytest
+from tests.test_server.test_app.views import DummyViewSetFixture
+
+
 @pytest.mark.action_api(view_set_class=DummyViewSetFixture)
 def test_call_as_api_fixture(db, action_api):
-    pass
+  pass
 ```
 Now you can use all `DummyViewSetFixture` functionality!
 
-#### Step 3: write your test
+#### Step 3: write your tests
 
 e.g:
 our ViewSet is called `DummyViewSetFixture`
-```python
-@pytest.mark.action_api(view_set_class=DummyViewSetFixture)
-def test_call_as_api_fixture(db, action_api):
-    dummy_model = DummyModel()
-    dummy_model.dummy_int = 1
-    dummy_model.save()
-    res = action_api.api_dummy(pk=1)
-    assert res["dummy_int"] == 1
-
-```
-
-### To use `drf-api-action` in your ViewSet, you need to follow these steps:
-
-#### Step 1: Import the Required Classes and Decorators
-
-Import the necessary classes and decorators from `drf-api-action` and `rest_framework`:
-
-```python
-from drf_api_action.decorators import action_api
-from drf_api_action.mixins import APIRestMixin
-from rest_framework.viewsets import ModelViewSet
-```
-
-#### Step 2: Inherit `APIRestMixin` in your View 
-
-Create your view class by inheriting the `APIRestMixin` class.
-
-For example, we want to inherit `ModelViewSet` (Could be any ViewSet) in our View:
-
-```python
-class DummyView(APIRestMixin, ModelViewSet):
-    queryset = DummyModel.objects.all()
-    serializer_class = DummySerializer
-```
-
-Another example:
 
 ```python
-class UsersViewSet(APIRestMixin, mixins.RetrieveModelMixin,
-                   mixins.ListModelMixin, viewsets.GenericViewSet):
-    serializer_class = UsersSerializer
-```
-
-#### Step 3: Define Your API Actions
+import pytest
+from tests.test_server.test_app.models import DummyModel
+from tests.test_server.test_app.views import DummyViewSetFixture
 
-Use the `action_api` decorator instead of `action` decorator to define your API actions as functions inside your view class:
 
-From:
-```python
-    @action(detail=True, methods=["get"], serializer_class=DummySerializer)
-    def dummy(self, request, **kwargs):
-        serializer = self.get_serializer(instance=self.get_object())
-        return Response(data=serializer.data, status=status.HTTP_200_OK)
-```
-
-To:
+@pytest.mark.action_api(view_set_class=DummyViewSetFixture)
+def test_call_as_api_fixture(db, action_api):
+  dummy_model = DummyModel()
+  dummy_model.dummy_int = 1
+  dummy_model.save()
+  res = action_api.api_dummy(pk=1)
+  assert res["dummy_int"] == 1
 
-```python
-    @action_api(detail=True, methods=["get"], serializer_class=DummySerializer)
-    def dummy(self, request, **kwargs):
-        serializer = self.get_serializer(instance=self.get_object())
-        return Response(data=serializer.data, status=status.HTTP_200_OK)
 ```
 
-In the example above, the `dummy` function is decorated with `action_api`.
-It specifies that the action requires a detail argument, supports the `GET` method, and uses the `DummySerializer` for serialization.
-
-#### Step 4: test REST methods
-
-* Create an instance of your view class and call the API actions as regular functions:
-
 ```python
-def test_dummy():
-    api = DummyView()
-    result = api.dummy(pk=1)
-    assert result['dummy_int'] == 1
-```
-
-*query parameters/post payload are treated as function arguments as kwargs*
+import pytest
+from tests.test_server.test_app.views import DummyViewSetFixture
 
 
-* Exceptions are raised explicitly:
-```python
-def test_dummy():
-    api = DummyView()
-    result = api.dummy(pk='bbb')
-    assert result['dummy_int'] == 1
+@pytest.mark.action_api(view_set_class=DummyViewSetFixture)
+def test_dummy(db, action_api):
+  result = action_api.dummy(pk='bbb')
+  assert result['dummy_int'] == 1
 ```
 
 ```shell
 tests/functionality_tests/test_as_api.py:11 (test_call_as_api)
 self = <django.db.models.fields.BigAutoField: id>, value = 'bb'
 
     def get_prep_value(self, value):
@@ -183,36 +149,21 @@
 >           return _get_object_or_404(queryset, *filter_args, **filter_kwargs)
 
 ../venv/lib/python3.9/site-packages/rest_framework/generics.py:19: 
 
 and so on....
 ```
 
-* Pagination support with `page`/`offset` kwarg (depends on `DEFAULT_PAGINATION_CLASS`):
-```python
->>> api = DummyAPIViewSet()
->>> response = api.by_dummy_int(request=None, dummy_int=1, page=2)
-
->>> {'count': 2, 'next': None, 'previous': '', 'results': [OrderedDict([('id', 2), ('dummy_int', 1)])]}
-
-```
 
 ## Package Testing
 
-The `drf-api-action` library includes tests to ensure the functionality works as expected. To run the tests, follow these steps:
-
-1. Navigate to the root directory of the `drf-api-action/` project.
-```shell
-cd tests/
-```
-
-2. Run the tests using `pytest`
+The `drf-api-action` library includes tests to ensure the functionality works as expected. To run the tests run `pytest`:
 
  ```shell
- python -m pytest -vv
+ pytest
  ```
 
 The tests will be executed, and the results will be displayed in the console.
 
 ## Example
 
 Example of using drf-api-action in a [DRF project](https://github.com/Ori-Roza/drf-api-action-example)
@@ -227,8 +178,9 @@
 
 ## Open an Issue
 
 For guidance on how to open an issue, see the [issue template](https://github.com/Ori-Roza/drf-api-action/blob/master/docs/ISSUE_TEMPLATE.md).
 
 ## Code Of Conduct
 
-[code of conduct](https://github.com/Ori-Roza/drf-api-action/blob/master/docs/CODE_OF_CONDUCT.md).
+[code of conduct](https://github.com/Ori-Roza/drf-api-action/blob/master/docs/CODE_OF_CONDUCT.md).
+
```

### Comparing `drf_api_action-1.1.0/drf_api_action/mixins.py` & `drf_api_action-1.2.0/drf_api_action/mixins.py`

 * *Files identical despite different names*

### Comparing `drf_api_action-1.1.0/pyproject.toml` & `drf_api_action-1.2.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,40 +1,66 @@
-[project]
+[build-system]
+requires = ["poetry_core>=1.0.0"]
+build-backend = "poetry.core.masonry.api"
+
+[tool.poetry]
 name = "drf_api_action"
+version = "1.2.0"
 description = "drf-api-action elevates DRF testing by simplifying REST endpoint testing to a seamless, function-like experience."
-version = "1.1.0"
 readme = "README.md"
-license = {file = "LICENSE.txt"}
-dependencies = ["Django>=4.2.8", "djangorestframework>=3.14.0", "pytest-django>=4.5.2", "pytest-cov>=4.1.0"]
-maintainers = [
-  { name="Ori Roza", email="ori75660@gmail.com" },
-]
-authors = [
-  { name="Ori Roza", email="ori75660@gmail.com" },
+authors = ["Ori Roza <ori75660@gmail.com>"]
+license = "MIT"
+repository = "https://github.com/Ori-Roza/drf-api-action"
+homepage = "https://github.com/Ori-Roza/drf-api-action"
+
+keywords = [
+  "pytest",
+  "mocks",
+  "testing",
+  "fixtures",
+  "tests",
+  "django"
 ]
-requires-python = ">=3.8"
+
+# Pypi classifiers: https://pypi.org/classifiers/
 classifiers = [
-    "Programming Language :: Python :: 3",
-    "License :: OSI Approved :: MIT License",
-    "Operating System :: OS Independent",
+  "Programming Language :: Python",
+  "Programming Language :: Python :: 3",
+  "Programming Language :: Python :: 3.7",
+  "Programming Language :: Python :: 3.8",
+  "Programming Language :: Python :: 3.9",
+  "Programming Language :: Python :: 3.10",
+  "Topic :: Software Development :: Testing",
+  'Framework :: Pytest',
+  "License :: OSI Approved :: MIT License",
+  "Development Status :: 5 - Production/Stable",
+  "Intended Audience :: Developers",
+  "Operating System :: OS Independent",
+]
+
+[tool.pytest.ini_options]
+DJANGO_SETTINGS_MODULE = "tests.test_server.settings"
+python_files = "tests.py test_*.py *_tests.py"
+markers = [
+    "action_api: Viewset"
 ]
+testpaths = ["tests"]
 
-[tool.setuptools]
-py-modules = []
+[tool.poetry.plugins.pytest11]
+api_action = "drf_api_action.plugin"
 
-[project.urls]
-Home-page = "https://github.com/Ori-Roza/drf-api-action"
-Documentation = "https://github.com/Ori-Roza/drf-api-action"
-"Source Code" = "https://github.com/Ori-Roza/drf-api-action"
-"Issue Tracker" = "https://github.com/Ori-Roza/drf-api-action/issues/"
 
+[tool.poetry.dependencies]
+python = "^3.7"
+importlib_metadata = {version = "^4.5.0", python = "<3.8"}
+Django = ">=4.2.8"
+djangorestframework = ">=3.14.0"
+pytest-django = ">=4.5.2"
+pytest-cov = "4.1.0"
 
-[build-system]
-build-backend = "flit_core.buildapi"
-requires = ["flit_core >=3.8.0,<4"]
 
 [tool.pylint.master]
 fail-under = 10.0
 ignore = [ "CVS",]
 ignore-paths = [ "tests", ".*test.*", ".*migrations.*",
   ".*requirements.*", ".*venv.*", ".*pyproject.*", ".*egg-info.*", ".*README.*"]
 jobs = 1
@@ -151,12 +177,7 @@
 [tool.pylint.imports]
 allow-wildcard-with-all = "no"
 analyse-fallback-blocks = "no"
 known-third-party = "enchant"
 
 [EXCEPTIONS]
 overgeneral-exceptions = [ "BaseException", "Exception",]
-
-[tool.pytest.ini_options]
-markers = [
-    "action_api",
-]
```

